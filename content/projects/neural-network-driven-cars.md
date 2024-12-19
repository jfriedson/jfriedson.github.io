---
date: 2022-05-01T00:00:00+05:00
draft: false
title: "Neural Network-Driven Cars"
---
## Neural Network-Driven Cars

This genetic algorithm crossbreeds and mutates world-class F1 drivers in your browser.

<a href="https://github.com/jfriedson/neural-network-cars" class="btn btn-primary" target="_blank" rel="noopener noreferrer"><i class="icon-github-line"></i>Source Code on GitHub</a>

You can load the trained network by clicking <button id="pretrained" class="btn btn-frameless" style="cursor: pointer;" title="Load Trained Network">here</button>. It completes the track but is quickly optimized. To learn more about how this project functions, please scoll down below the demo.

<div id="project-iframe-container" class="d-flex justify-content-center flex-nowrap"><iframe src="/projects/neural-network-cars/app" title="Gentic Cars Demo" frameborder="0" scrolling="no"></iframe></div>

<br />
<h5>About the Architecture</h5>
<div style="padding-left: 20pt">
    <h6>Neural Networks</h6>
    <p>The neural networks driving each car have the following attributes:</p>
    <ul>
        <li>13 inputs - 7 forward and side-facing distance sensors and the car's speed, angular velocity, steerings angle, gas throttle, and standard and emergency brakes</li>
        <li>1 hidden layer of 10 neurons - found to be a good balance of training time and function complexity for this simple problem</li>
        <li>4 outputs - steerings angle, gas throttle, and standard and emergency brakes</li>
    </ul>
    <p>
        Each input is normalized to enhance the genetic algorithm's performance.
        The network applies leakyRELU activation on the hidden layer and sigmoid activation on the output.
        The network outputs are then denormalized and applied to the physical body of the car.
    </p>
    <h6>Genetic Algorithms</h6>
    <p>
        There are 3 different genetic algorithms that take turns acting on the neural networks in a round robin fashion. 
        They differ in how they introduce new genetics to the genome pool through the use of mutation and cross-breeding. 
        Two algorithms splice new, random neurons into the best performing networks, while the third cross-breeds and mutates only the champion networks.
    </p>
</div>
