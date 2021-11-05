# onlinecviceni-solver
script do console který vyplní políčka ve cvičeních na onlinecviceni.cz

# kód pro slovní doplnění (funguje pro většinu matematických cvičení)
```js
var ff = document.getElementById("id_form2").firstElementChild
var v = ff.value.split("%3B")
var vecii = []
for(let i =-1;i<ff.value.split("%3B").length-1;i+=2) {
  vecii.push(v[i])
}
for(var o=1;o<vecii.length;o++) {
  ro = o
  console.log(ro, vecii[ro])
  	if(vecii[ro].includes("%")) {
  		document.getElementById("idField"+(ro-1).toLocaleString()).value = decodeURIComponent(vecii[ro]  )
    } else {
  		document.getElementById("idField"+(ro-1).toLocaleString()).value = vecii[ro]  
    }
}
```

# kód pro výběr z nabídky (funguje pro většinu češtinářských cvičení)
```js
// zatím není...
```
