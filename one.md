setcpm(80/4)

$: sound("[numbers:1 ~ ~ ~] / 2 [numbers:2 ~ ~ ~] / 2")

$: sound(`
[hh hh -  hh ]  [hh:3 -  hh hh ] [hh -  hh hh ] [hh [hh hh:3]  hh hh * 2 ],
[-  -  oh - ]  [-  -  -  - ] [-  -  -  oh ] [-  -  -  - ],
[-  -  cp  - ]  [cp -  -  - ] [-  -  -  - ] [cp -  -  - ],
[-  -  -  rim] [-  -  -  rim] [- rim -  - ] [-  -  rim rim],
[-] [-] [-] [-]
`)

$: note("<[[d3,a3,f4] ~@15] [[d3,bb3,g4] ~@15] [[bb3,d4,f4] ~@15] [[a3,c#4,e4] ~@15]>")
  .attack(0.25)
  .sustain(0.25)
  .release(0.25)
.sound("sawtooth")
.lpf(5000)
