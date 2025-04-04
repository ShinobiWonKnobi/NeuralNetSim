# Neural Network Digit Recognition Simulator

An interactive, visual neural network simulator that demonstrates how artificial neural networks (ANNs) learn to recognize handwritten digits. This single-file HTML application provides a hands-on way to build intuition about neural network behavior.

## Features

- **Interactive Visualization**: See the network's neurons and connections in real-time as it processes input
- **Weight Visualization**: Hover over hidden neurons to visualize what features they're detecting
- **Test Mode**: Draw your own digits and see if the network can recognize them
- **Parameter Controls**: Experiment with:
  - Learning rate
  - Hidden neuron count
  - Activation functions (Sigmoid, ReLU)
  - Input noise
- **Training Metrics**: Monitor training error and accuracy over time
- **Save/Load**: Store trained network weights in browser local storage

## How to Use

1. **Open the file**: Simply open `neuronn.html` in any modern web browser
2. **Read the documentation**: Click "What is this?" to understand the components
3. **Train the network**: 
   - Click "Start Training" to begin automatic training
   - Use "Step Once" to advance one training example at a time
   - Monitor the error graph to see progress
4. **Test the network**:
   - Click "Enter Test Mode" once training progress looks good
   - Draw a digit on the grid
   - Click "Predict Drawn Digit" to see the network's prediction

## Understanding the Visualization

- **Input Grid**: Shows the current digit pattern (5×7 grid)
- **Network Diagram**: 
  - Shows neurons (circles) with activation levels (brightness)
  - Shows weights (connections) with sign (blue = positive, red = negative) and strength (opacity/thickness)
- **Hidden Neuron Weights**: Reveals what patterns each hidden neuron is detecting
- **Gradient Visualization**: Option to highlight which connections are being updated during backpropagation

## Technical Details

The simulator implements:
- A fully-connected feedforward neural network (35-input, variable hidden layer, 10-output)
- Backpropagation learning algorithm with gradient descent
- Choice of activation functions (Sigmoid, ReLU)
- Mean Squared Error (MSE) loss function
- Optional noise injection for improved generalization

## Experimentation Ideas

- Try different learning rates and observe convergence behavior
- Compare how ReLU vs Sigmoid activation affects learning
- See how increasing/decreasing hidden neurons impacts learning capacity
- Add noise during training and test if it improves generalization
- Examine which hidden neurons detect similar features

## Browser Compatibility

Tested and works with:
- Chrome (recommended)
- Firefox
- Edge
- Safari

## License

MIT License - Feel free to use, modify and distribute!
