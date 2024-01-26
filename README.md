# Self-Driving Car Simulation using Neural Networks

This repository hosts the JavaScript implementation for a self-driving car simulation employing neural networks and sensors to navigate through traffic and adhere to road borders. The objective is to develop an autonomous driving system driven by an efficient AI.

## Overview

Constructed using vanilla JavaScript, the self-driving car relies on neural networks to make decisions. The neural network serves as the car's brain, enabling it to navigate through traffic, avoid collisions, and stay within road boundaries.

## Neural Network Optimization

The system adopts an iterative optimization approach. Multiple AI-powered brains are concurrently tested to identify the most effective configuration, enhancing the decision-making capabilities of the car over time.

## Simulation Models

The code structure supports multiple simulation models of the car, each associated with a unique brain identifier. These simulations involve the car navigating its environment based on feedback from the neural network. With each iteration, the car learns from its experiences, continuously improving its ability to avoid collisions and maintain forward momentum.

## Persistent Learning

A crucial feature of the simulation is the ability to save the most effective brain identifier using a designated save button. Users can persistently store and refine the most successful neural network configuration over time.

## Getting Started

To experience the self-driving car simulation live, open the code on the web. Interact with the simulation, save the optimal brain configuration, and observe the continuous improvement of the car's autonomous capabilities.

## Project Structure
index.html: Connects all JavaScript files together and provides the interface for the live simulation.
JavaScript Files:
car.js: Defines the car object and its behavior within the simulation.
controls.js: Manages user input controls and interactions with the simulation.
network.js: Implements the neural network responsible for decision-making in the self-driving car.
road.js: Handles the representation and behavior of the road within the simulation.
main.js: Contains the core logic for the self-driving car, including the integration of various components.
sensor.js: Implements sensors to capture and process environmental data for the neural network.
utils.js: Houses utility functions and helper methods used across different parts of the simulation.
visualizer.js: Manages the visual representation of the simulation, aiding in debugging and analysis.
Style and Visualization:
styles.css: Provides styling to enhance the visual representation of the simulation

## Implementation Details (main.js excerpt)

Within the `main.js` file, you'll find the following code snippet:

const N = 1;  // Represents the best brain
const cars = generateCars(N);
let bestCar = cars[0];

The `N` constant signifies the best brain configuration. You can adjust this number to allow the car to learn from additional brains, but keep in mind that the optimal value depends on your PC's processing power. Experiment with different values to find the right balance between learning capacity and computational resources.
