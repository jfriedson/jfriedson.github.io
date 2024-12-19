---
date: 2024-12-04T00:00:00-08:00
draft: false
title: "MNIST Go + Electron + React App"
---
## MNIST Go + Electron + React App

An Electron app using React for UI accepts user-created MNIST digit images using an HTML Canvas and sends the input to a Go service for neural network inference.  The Go service implements multiple goroutine accelerated strategies for the neural network layers that have been benchmarked and analyzed on the <a href="https://github.com/jfriedson/mnist-go-electron-react-app/tree/master/go-service">GitHub project page</a>. The neural network's prediction is then returned to the React UI and displayed to the user.

<a href="https://github.com/jfriedson/mnist-go-electron-react-app/" class="btn btn-primary" target="_blank" rel="noopener noreferrer"><i class="icon-github-line"></i>Source Code on GitHub</a>

<a rel="noopener noreferrer" href="https://raw.githubusercontent.com/jfriedson/mnist-go-electron-react-app/master/showcase.webp"><img class="project-pic" src="https://raw.githubusercontent.com/jfriedson/mnist-go-electron-react-app/master/showcase.webp" alt="Animated demo of MNIST Go + Electron + React App" style="max-width: 100%;"></a>
