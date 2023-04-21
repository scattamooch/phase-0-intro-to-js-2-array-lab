const cats = ["Milo", "Otis", "Garfield"]
beforeEach(function () {
    cats.length = 0;
  
    cats.push("Milo", "Otis", "Garfield");
  });

function destructivelyAppendCat() {
    cats.push("Ralph")
    return destructivelyAppendCat
}
function destructivelyPrependCat() {
    cats.unshift("Bob")
    return destructivelyPrependCat
}
function destructivelyRemoveLastCat() { 
    cats.pop()
    return destructivelyRemoveLastCat
}
function destructivelyRemoveFirstCat() {
    cats.shift()
    return destructivelyRemoveFirstCat
}
function appendCat() {
    appendCat = [...cats, "Broom"]
    return appendCat
}

function prependCat() {
    prependCat = ["Arnold",...cats]
    return prependCat
}
function removeLastCat() { 
    removeLastCat = cats.slice(0,2)
    return removeLastCat
}
function removeFirstCat() {
    removeFirstCat = cats.slice(-2)
    return removeFirstCat
}