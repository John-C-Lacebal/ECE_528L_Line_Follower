# ECE 528/L - Robotics and Embedded Systems with Lab
**CSU Northridge**

**Department of Electrical and Computer Engineering**

## Line Follower Lab
The Line Follower lab interfaces with the following:

* User LEDs of the TI MSP432 LaunchPad
* Pololu Gearmotor with Encoder - [Product Link](https://www.pololu.com/product/3675)
* 8-Channel QTRX Sensor Array - [Product Link](https://www.pololu.com/product/3672)

Pre-Lab

1. 
````c
void Chassis_Board_LEDs_Init()
{

}
````

2. 
````c
void Print_Tenth()
{
    for (int i = 10; i <= 51; i++) {
        if ((i % 10) == 0) {
            printf(“Index %d: Every 10th iteration.\n”, i);
        } else if ((i % 10) == 1) {
            printf(“Index %d: Following the 10th iteration.\n.”, i);
        }
    }
}
````