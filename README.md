# X2-Coin-Flip-
input.onGesture(Gesture.Shake, function () {
    CoinAHeads = Math.randomBoolean()
    CoinBHeads = Math.randomBoolean()
    if (CoinAHeads == CoinBHeads) {
        basic.showLeds(`
            . # # # .
            # . . . #
            # # # # #
            # . . . #
            # . . . #
            `)
        basic.pause(100)
        PlayerAScore += 1
    } else {
        basic.showLeds(`
            # # # # .
            # . . . #
            # # # # #
            # . . . #
            # # # # .
            `)
        basic.pause(100)
        PlayerBScore += 1
        basic.showLeds(`
            . # . . .
            # # # . .
            . # . # .
            . . # # #
            . . . # .
            `)
    }
})
input.onButtonPressed(Button.A, function () {
    CoinAHeads = Math.randomBoolean()
    CoinBHeads = Math.randomBoolean()
    PlayerAScore = 0
    PlayerBScore = 0
    basic.showLeds(`
        . # . . .
        # # # . .
        . # . # .
        . . # # #
        . . . # .
        `)
})
let CoinBHeads = false
let CoinAHeads = false
let PlayerBScore = 0
let PlayerAScore = 0
PlayerAScore = 0
PlayerBScore = 0
CoinAHeads = false
CoinBHeads = false
basic.showLeds(`
    . # . . .
    # # # . .
    . # . # .
    . . # # #
    . . . # .
    `)
