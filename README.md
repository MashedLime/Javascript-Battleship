# Javascript-Battleship
Just a short game to play on a javascript console.
Go to the code section for the proper javascript code.

let ship1 = Math.floor(Math.random()* 98)+ 2
let ship2 = ship1 - 1
let ship3 = ship1 + 1
let hitCount = 0
let torpedo = 0

while(hitCount < 3){
    torpedo = prompt("Guess a number from 1 to 100!")
    if(torpedo == ship1){
        console.log("Hit!")
        hitCount = hitCount + 1
        ship1 = -1
    }else if(torpedo == ship2){
        console.log("Hit!")
        hitCount = hitCount + 1
        ship2 = -1
    }else if(torpedo == ship3){
        console.log("Hit!")
        hitCount = hitCount + 1
        ship3 = -1
    }else{
        console.log("Miss!")
    }
}

console.log("You sunk the battleship! You win!")
