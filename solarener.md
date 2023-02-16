# Solar Energy 

```package
cakEnergy=github:climate-action-kits/pxt-climate-action-kit-energy
```
## @showhint
Create a ``||Variables:Variable position||`` and nest ``||Variables:set position to -90||`` 
under ``||basic:on start||`` block
```blocks
let position = -90
```

## @showhint
Now add ``||cakLandServos:turn right motor + pin on||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
```
## @showhint
Now nest an ``||logic:If true then else||`` block under the ``||basic:forever||`` loop
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(true){
    }
    else{
    }
})
```
## @showhint
Add a ``||logic:comparison block||`` from the ``||logic:Logic drawer||`` place it in the true
condition of the ``||logic: if then else||`` loop
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(||){
    }
    else{
    }
})
```
## @showhint
Insert the block ``||cakLandLight:light level at pin P1 is Intense||`` under ``||i||``
and insert ``||cakLandLight:light level at pin P1 is Bright||`` under ``||j||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright))){
    }
    else{
    }
})
```
## @showhint
If the condition is true add ``||basic:show icon||`` block and select ``||basic:target icon||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    }
})
```
## @showhint
If the condition is false add ``||basic:show icon||`` block under the ``||logic:else||`` and select ``||basic: small diamond icon||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    }
})
```

## @showhint
Now add ``||Variables:change position by 10||`` block under the ``||basic:small diamond icon||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    position += 10
    }
})
```

## @showhint
Add ``||logic:if true then||`` block under the ``||logic:else||`` condition below the ``||Variables:change position by 10||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    position += 10
        if(true){
        }
    }
})
```
## @showhint
For the true condition replace it by a ``||logic:comparison||`` block
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    position += 10
        if(>){
        }
    }
})
```
## @showhint
For the comparison add ``||Variables:position||`` on the left side and compare with ``||90||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    position += 10
        if(position>90){
        }
    }
})
```
## @showhint
For the true condition add ``||Variables:set position to -90||`` nested under the ``||logic:if position>90 then||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    position += 10
        if(position>90){
        position = -90
        }
    }
})
```
## @showhint
Add ``||cakLandServos: turn servo at P8 to degrees:||`` and ``||Variables:position||`` block after the ``||logic:if then||`` block
Also add a ``||basic:pause||`` block and set it to ``||basic:20ms||``
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function(){
    if(cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)){
    basic.showIcon(IconNames.Target)
    }
    else{
    basic.showIcon(IconNames.SmallDiamond)
    position += 10
        if(position>90){
        position = -90
        }
        cakLandServos.turnServo(cakLandServos.ServoPin.P8, position)
        basic.pause(20)
    }
})
```
## @showhint
This is the final code
```blocks
let position = -90
cakLandServos.motorPinPower(cakLandServos.MotorPin.Right, cakLandServos.Power.On)
basic.forever(function () {
    if (cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Intense) || cakLandLight.ifLuminance(cakLandLight.LightPin.P1, cakLandLight.Luminance.Bright)) {
        basic.showIcon(IconNames.Target)
    } else {
        basic.showIcon(IconNames.SmallDiamond)
        position += 10
        if (position > 90) {
            position = -90
        }
        cakLandServos.turnServo(cakLandServos.ServoPin.P8, position)
        basic.pause(20)
    }
})
```