PermissionsEXSquish
===================

This is for Squishbum

groups:
  Newb:
    default: true
    prefix: ' '
    permissions:
    - MasterPromote.member
    - group.<Newb>
    - multiverse.portal.access.hg1
    - multiverse.portal.access.hg1leave
    - multiverse.portal.access.wilderness1
    - multiverse.portal.access.flatworld
    - multiverse.portal.access.spawnportal
    - multiverse.portal.access.SpawnC
    - multiverse.portal.access.DiamondPortal
    - sg.arenas.join.5
    - sg.arenas.join.3
    - sg.arena.join
    - sg.lobby.join
    - sg.arena.vote
    - sg.arena.spectate
    - essentials.afk
    - essentials.home
    - modifyworld.*
    - essentials.list
    - essentials.rules
    - essentials.spawn
    - essentials.tpaccept
    - essentials.tpdeny
    - essentials.tpa
    - essentials.mail
    - essentials.sethome
    - essentials.mail.send
    - essentials.balance
    - essentials.msg
    - essentials.back.ondeath
    - essentials.sign.use
    - essentials.signs.use.warp
    - essentials.signs.use.sell
    - essentials.signs.use.buy
    - essentials.signs.use.heal
    - craftbook.mech.gate.use
    - craftbook.mech.bridge.use
    - craftbook.mech.elevator.use
    - essentials.clearinventory
    inheritance:
    - null
    options:
      rank: '1000'
      build: true
      suffix: ''
  CoalMiner:
    default: false
    prefix: '&8Coal Miner&f> '
    permissions:
    - group.<Builder>
    - essentials.sethome
    - essentials.signs.use.kit
    - essentials.kit
    - essentials.me
    - essentials.delhome
    - plotme.use
    - plotme.use.add
    - plotme.use.remove
    - plotme.limit.1
    inheritance:
    - Newb
    options:
      rank: '900'
      build: true
      suffix: ''
  IronMiner:
    default: false
    prefix: '&7Iron Miner&f> '
    permissions:
    - essentials.back
    - essentials.sign.use.*
    - craftbook.mech.elevator
    - craftbook.mech.bridge
    - craftbook.mech.gate
    - essentials.workbench
    - essentials.enderchest
    - essentials.sethome.multiple.2
    inheritance:
    - CoalMiner
    options:
      rank: '800'
      build: true
      suffix: ''
  RedstoneMiner:
    default: false
    prefix: '&4Redstone Miner&f> '
    permissions:
    - essentials.back
    - essentials.sign.use.*
    - craftbook.mech.elevator
    - craftbook.mech.bridge
    - craftbook.mech.gate
    - essentials.workbench
    - essentials.enderchest
    - essentials.sethome.multiple.2
    inheritance:
    - IronMiner
    options:
      rank: '750'
      build: true
      suffix: ''
  YouTube:
    default: false
    prefix: '&fYou&4&lTuber&f> '
    permissions:
    - essentials.back
    - essentials.sign.use.*
    - craftbook.mech.elevator
    - craftbook.mech.bridge
    - craftbook.mech.gate
    - essentials.workbench
    - essentials.enderchest
    - essentials.sethome.multiple.2
    inheritance:
    - IronMiner
    options:
      rank: '750'
      build: true
      suffix: ''
  Donator:
    default: false
    prefix: '&f[&4Donator&f]'
    permissions:
    - essentials.fly
    inheritance:
    - RedstoneMiner
  Moderator:
    default: false
    prefix: '&3[&5Moderator&3]&f'
    permissions:
    - essentials.ban
    - essentials.ban.offline
    - essentials.tempban
    - essentials.tempban.offline
    - essentials.unban
    - essentials.tp
    - essentials.chat.url
    - essentials.signs.color
    - essentials.joinfullserver
    - essentials.feed
    - essentials.sethome.multiple.3
    - essentials.kick
    inheritance:
    - Donator
    options:
      rank: '700'
      build: true
      suffix: ''
  Admin:
    default: false
    prefix: '&f[&cAdmin&f] '
    permissions:
    - essentials.ignore
    - essentials.hat
    - essentials.signs.color
    - essentials.chat.color
    - essentials.fly
    - essentials.fly.safelogin
    - essentials.repair
    - essentials.heal
    - essentials.top
    - essentials.mute
    inheritance:
    - Moderator
    options:
      rank: '600'
      build: true
      suffix: ''
  Head-Admin:
    default: false
    prefix: '&f[&6Head-Admin&f] '
    permissions:
    - vanish.*
    - essentials.god
    - essentials.keepxp
    - essentials.jump
    - simplesignedit.edit
    inheritance:
    - Admin
    options:
      rank: '500'
      build: true
      suffix: '[&5o&lSamfluffy&f]'
  Monster:
    default: false
    prefix: '&2[&4Mon&2ster&4]&f'
    inheritance:
    - Admin
    options:
      rank: '400'
      build: true
      suffix: ''
  Ghost:
    default: false
    prefix: '&4[&7Ghost&4]&f'
    inheritance:
    - Head-Admin
    options:
      rank: '300'
      build: true
      suffix: ''
  Co-Owner:
    default: false
    prefix: '&5[&6Co-Owner&5]&f '
    permissions:
    - '*'
    inheritance:
    - Head-Admin
    options:
      rank: '200'
      build: true
      suffix: ''
  Owner:
    default: false
    prefix: '&6[&bOwner&6] '
    permissions:
    - '*'
    inheritance:
    - Co-Owner
    options:
      rank: '100'
      build: true
      suffix: ''
users:
  squishbum:
    group:
    - Owner
