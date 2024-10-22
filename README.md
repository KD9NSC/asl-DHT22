# DHT22
Slightly modified version of [DHT22 by wookookie](https://github.com/wookookie/DHT22) for easy parsing in bash.

## How to clone
1. Open the terminal in Raspbian.
2. Check your Git installation.
```
$ sudo apt-get install git-core
```
3. Enter a clone command with this repository address.
```
$ git clone https://github.com/ccoong7/DHT22.git
```

## How to create an executable file
1. When clone success, change directory to DHT22.
```
$ cd ~/DHT22
```
2. Compile source code to generate an executable file.
```
$ gcc -o dht22.out dht22.c -lwiringPi
```
3. Launch!
```
$ ./dht22.out
```
![result](/resources/dht22_result.png)

## Wiring
- Vcc 3.3V
- Signal pin is GPIO 18 (With 5k resistor or 10k parallel)
- 3rd pin is not used
- GND
![wiring](/resources/dht22_wiring.png)
