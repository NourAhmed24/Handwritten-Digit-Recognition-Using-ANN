<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Project README View</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            margin: 40px;
            background-color: #f6f8fa;
        }
        .readme-container {
            max-width: 900px;
            margin: 0 auto;
            padding: 30px;
            background-color: #ffffff;
            border: 1px solid #e1e4e8;
            border-radius: 6px;
            box-shadow: 0 1px 3px rgba(27,31,35,.1);
        }
        h1 {
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
            font-size: 2em;
        }
        h2 {
            border-bottom: 1px solid #eaecef;
            padding-bottom: 0.3em;
            font-size: 1.5em;
            margin-top: 30px;
        }
        code {
            background-color: #f3f4f6;
            padding: 2px 5px;
            border-radius: 3px;
        }
        pre {
            background-color: #f3f4f6;
            padding: 16px;
            overflow: auto;
            line-height: 1.45;
            border-radius: 6px;
        }
        table {
            border-collapse: collapse;
            width: 100%;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #dfe2e5;
            padding: 8px 13px;
            text-align: left;
        }
        th {
            background-color: #f6f8fa;
        }
    </style>
</head>
<body>

<div class="readme-container">
    <h1>✍️ Handwritten Digit Recognition Using ANN</h1>

  <h2>Description</h2>
    <p>This project tackles the classic problem of <strong>Handwritten Digit Recognition</strong> using an <strong>Artificial Neural Network (ANN)</strong>, specifically implemented as a <strong>Multi-Layer Perceptron (MLP)</strong>. It serves as a fundamental introduction to image classification, demonstrating how simple neural architectures can achieve high performance on complex, real-world data.</p>
    <p>The model is trained on the widely-used <strong>MNIST dataset</strong>, which consists of 60,000 training and 10,000 testing examples of $28 \times 28$ pixel grayscale images of handwritten digits (0 through 9). The core goal is to build, train, and evaluate a neural network capable of accurately identifying and classifying any given handwritten digit image.</p>

  <h2>✨ Key Features</h2>
    <ul>
        <li><strong>Architecture:</strong> Uses a fully connected <strong>Multi-Layer Perceptron (MLP)</strong>.</li>
        <li><strong>Dataset Handling:</strong> Implementation includes loading, normalizing, and flattening the 28x28 image data.</li>
        <li><strong>Training:</strong> Utilizes core machine learning concepts like <strong>backpropagation</strong>, <strong>gradient descent</strong>, and categorical cross-entropy loss.</li>
        <li><strong>Evaluation:</strong> Tracks performance metrics such as accuracy and loss curves.</li>
        <li><strong>High Performance:</strong> Achieves a classification accuracy typically <strong>exceeding 95%</strong> on the test set.</li>
    </ul>

  <h2>⚙️ Technologies Used</h2>
    <table>
        <thead>
            <tr>
                <th>Technology</th>
                <th>Purpose</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Python</strong></td>
                <td>Primary development language.</td>
            </tr>
            <tr>
                <td><strong>TensorFlow / Keras</strong></td>
                <td>Framework for building and training the neural network.</td>
            </tr>
            <tr>
                <td><strong>NumPy</strong></td>
                <td>Efficient numerical and array operations for data handling.</td>
            </tr>
            <tr>
                <td><strong>Matplotlib</strong></td>
                <td>Visualization of digits, training progress, and results.</td>
            </tr>
        </tbody>
    </table>

  <h2>🚀 Getting Started</h2>
    <p>Follow these steps to set up and run the project locally:</p>

   <h3>Prerequisites</h3>
    <p>You need Python 3.x installed on your system.</p>

  <h3>Installation</h3>
    <ol>
        <li><strong>Clone the repository:</strong>
            <pre><code>git clone [your-repository-link-here]
cd handwritten-digit-recognition-ann</code></pre>
        </li>
        <li><strong>Install dependencies:</strong>
            <pre><code>pip install -r requirements.txt</code></pre>
        </li>
    </ol>

  <h3>Execution</h3>
    <p>Run the main training script. This will load the MNIST data, build the model, train it, and print the final evaluation accuracy.</p>
    <pre><code>python train_model.py</code></pre>

  <h2>💡 Model Architecture Overview</h2>
    <p>The MLP typically consists of:</p>
    <ol>
        <li><strong>Input Layer:</strong> 784 nodes (corresponding to 28x28 flattened pixels).</li>
        <li><strong>Hidden Layer(s):</strong> One or more dense layers (e.g., 128 nodes) with the <strong>ReLU</strong> activation function.</li>
        <li><strong>Output Layer:</strong> 10 nodes (for digits 0-9) with the <strong>Softmax</strong> activation function to get classification probabilities.</li>
    </ol>
</div>

</body>
</html>
