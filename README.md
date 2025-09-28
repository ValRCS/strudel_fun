# strudel_fun
Experiments with Strudel computational live music platform


## Deep Acid from Switch Angel recreation

Recreation of Switch Angel's famous track:
https://www.youtube.com/watch?v=HkgV_-nJOuE

Some extra controls: https://strudel.cc/#JDogcygic2JkITQiKS5fc2NvcGUoKS5kdWNrKCIyOjM6NCIpLmR1Y2thdHRhY2soLjIpLmR1Y2tkZXB0aCguOCkKCiRiYXNzOiBuKGlyYW5kKDEwKS5zdWIoNykuc2VnKDE2KSkuc2NhbGUoImM6bWlub3IiKQogIC5yaWIoNDYsMSkuZGlzdG9ydCgiMi4yOi4zIikKLnMoInNhd3Rvb3RoIikubHBmKDIwMCkubHBlbnYoc2xpZGVyKDIuNTI4LDAsOCkpLmxwcSgxMikKLm9yYml0KDIpLl9waWFub3JvbGwoKQoKJDogcygic3VwZXJzYXciKS5kZXR1bmUoMSkucmVsKDUpLmJlYXQoMiwzMikuc2xvdygyKQoub3JiaXQoMikuZm0oIjIiKS5mbWgoMi4wNCkKCiQ6IHMoInB1bHNlIikub3JiaXQoc2xpZGVyKDQsMCw0KSkuc2VnKHNsaWRlcigxNiwwLDE2KSkuZGVjKC4xKS5mbSh0aW1lKS5mbWgodGltZSkK

`
$: s("sbd!4")._scope().duck("2:3:4").duckattack(.2).duckdepth(.8)

$bass: n(irand(10).sub(7).seg(16)).scale("c:minor")
  .rib(46,1).distort("2.2:.3")
.s("sawtooth").lpf(200).lpenv(slider(2.528,0,8)).lpq(12)
.orbit(2)._pianoroll()

$: s("supersaw").detune(1).rel(5).beat(2,32).slow(2)
.orbit(2).fm("2").fmh(2.04)

$: s("pulse").orbit(slider(4,0,4)).seg(slider(16,0,16)).dec(.1).fm(time).fmh(time)
`
