# Parallel and Series Equivalent Load Value Calculator (Resistors, Inductors, Capacitors)

Author: Nathan Ng\
Date Created: November 17, 2019\
Current Version: V3

*Note 1: This is a WIP repository.*\
*Note 2: This repository is compiled in Eclipse IDE.*

## Features

* Parallel and Series equivalent load calculations, supporting a single load type (resistor, capacitor, inductor).
* Solves all equivalent load values of the circuit based on how the user wants their loads connected.
* Labels all resistor connections as an equation for all the equivalent loads and equivalent load values of the entire circuit.
* Console-based UI.


## Instructions

![Sample Circuit Diagram with Resistance Equations](https://raw.githubusercontent.com/Nathanyhang/SimpleResistanceCalculator/master/images/Circuit%20Diagram.png)
*Figure 1: Sample circuit diagram with load equations and sample input from the program. The green text are sample commands of what you would type in the console to "build" a circuit.*


**_The main program of this project is labelled as CircuitCalculator.java, located in src._**
1. Enter your list of load values **in order** as the load IDs are automatically labelled with respect to the order of your input.
2. Enter your load connections in the following format:

		ID ID ID ConnectionType

  	*where ID is your load ID and ConnectionType is either denoting a Parallel or Series circuit, for example:*

		R1 R2 R3 P
		R1 R2 R3 Parallel

    *both statements represent R1//R2//R3. To add circuits, use the same format and given IDs from the console.*

3. Type "end" when you have completed all connections.
4. The following will be displayed as output:
	* Equivalent resistance in ohms, farads, or henries.
	* All load IDs and their respective values.
	* Final equivalent load equations with "//" denoting Parallel and "+" denoting Series.
	* All generated load equations while the user is entering their circuit connections.
