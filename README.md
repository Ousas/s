SpawnG:
  Type: ARMOR_STAND
  Display: '&f[&lWITCH&f] &a☣  &f[&aLv.&c3&f]'
  Options:
    AlwaysShowName: true
#    MovementSpeed: 0.2
    Marker: true
    Invisible: false
  Skills: 
  - skill{s=SpawnG} @Self ~onSignal:Goodboy
GoodBoy:
  Type: WITCH
  Display: '&f[&lWITCH&f] &a☣  &f[&aLv.&c3&f]'
  Health: 25
  Damage: 14
  Options:
    AlwaysShowName: true
    MovementSpeed: 0.2
  Skills: 
  - modifyglobalscore{obj=GoodBoy;a=set;value=0} ~onDesth
