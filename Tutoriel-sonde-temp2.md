# Tutoriel-sonde-temp2
# Sonde de temperature-Tutoriel



## Step 1

Programme le MicroBit pour affiche les valeurs de la sonde de temperature DS18B20

## Step 2

Suprimme de le bloc ``||basic:au démarrage||``.


## Step 3

Cree une variable avec le bloc ``||let item: temperature|`` dans l'onglet  ``||variable|``
## Step 4

Ajoute le bloc ``||definir temperature = 0|`` dans le bloc  ``||basic.toujours|``

```blocks 

 

let temperature = 0
basic.forever(function () {
    temperature = 0
})


 

``` 
## Step 5

Ajoute l'extention DS18B20  et selectionne le bloc ``||dstemp.celsius(DigitalPin.P0)|`` et place le dans le bloc  ``||definir temperature = 0|`` 
```blocks 


let temperature = 0
basic.forever(function () {
    temperature = dstemp.celsius(DigitalPin.P0)
})


``` 
## Step 6

Ajoute le bloc ``||if (true) { }|``.

## Step 7

Ajoute le bloc ``||if (0 > 0) { }|``  le bloc  ``||if (true) { }|``.

```blocks 


let temperature = 0
basic.forever(function () {
    temperature = dstemp.celsius(DigitalPin.P0)
    if (0 > 0) {
    	
    }
})



``` 

## Step 8

Remplace le premier 0 de la comparaison avec le bloc  ``||temperature|`` et remplace le 2e 0 de la comparaison par la valeur -300. 

```blocks 


let temperature = 0
basic.forever(function () {
    temperature = dstemp.celsius(DigitalPin.P0)
    if (temperature > -300) {
    	
    }
})



```


## Step 9

Ajoute le bloc  ``||basic.showNumber(value,interval)|`` et remplace le 0 par le bloc  ``||temperature|`` .


```blocks 

let temperature = 0
basic.forever(function () {
    temperature = dstemp.celsius(DigitalPin.P0)
    if (temperature > -300) {
        basic.showNumber(temperature)
    }
})



``` 

## Step 10
Ajoute le bloc  ``||basic.pause(ms)|`` et remplace le 0 par la valeur ``||2000|`` .


```blocks 

let temperature = 0
basic.forever(function () {
    temperature = dstemp.celsius(DigitalPin.P0)
    if (temperature > -300) {
        basic.showNumber(temperature)
        basic.pause(2000)
    }
})




``` 
## Step 11

Réalise le branchement ci-dessous. 


La couleur des fils n'a pas d'importance! 

## @showdialog 

 

Félicitations!Tu as terminé de programmer la sonde de temperature DS18B20
 

Pour tester la sonde télécharge la programmation dans le micro:bit. 