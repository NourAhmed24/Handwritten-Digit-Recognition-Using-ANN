<!DOCTYPE html>
<html lang="en">

<body>

   <h1>✍️ Handwritten Digit Recognition using Artificial Neural Networks (ANN)</h1>
    
   <p>This project implements a simple yet effective <strong>Artificial Neural Network (ANN)</strong> model using <strong>TensorFlow/Keras</strong> to classify handwritten digits (0-9). The model is trained on the classic MNIST-like dataset containing 42,000 samples.</p>

   <hr>

   <h2>🚀 Key Features</h2>
    <ul>
        <li><strong>Model Architecture:</strong> A fully connected (Dense) Neural Network.</li>
        <li><strong>Framework:</strong> Built using <code>tensorflow.keras</code>.</li>
        <li><strong>High Accuracy:</strong> Achieved a <strong>~97%</strong> validation accuracy.</li>
    </ul>

   <hr>

   <h2>⚙️ Technical Details</h2>

   <h3>Dataset & Preprocessing</h3>
    <ul>
        <li><strong>Source:</strong> A CSV file (<code>Train.csv</code>) containing <strong>42,000</strong> samples of handwritten digits <span class="citation"></span>.</li>
        <li><strong>Image Format:</strong> Each image is <strong>28x28</strong> pixels, flattened to a <strong>784-feature</strong> vector <span class="citation"></span>.</li>
        <li><strong>Preprocessing Steps:</strong>
            <ul>
                <li>Pixel values normalized to the range <strong>[0, 1]</strong> <span class="citation"></span>.</li>
                <li>Labels are converted using <strong>One-Hot Encoding</strong> <span class="citation"></span>.</li>
                <li>Data is split into 80% training and 20% testing/validation sets <span class="citation"></span>.</li>
            </ul>
        </li>
    </ul>

   <h3>Model Architecture (ANN)</h3>
    <p>The model is a <code>Sequential</code> ANN with the following layers <span class="citation"></span>:</p>

   <table>
        <thead>
            <tr>
                <th>Layer Type</th>
                <th>Output Shape</th>
                <th>Activation</th>
                <th>Trainable Parameters</th>
            </tr>
        </thead>
    <tbody>
            <tr>
                <td><strong>Flatten</strong></td>
                <td>(None, 784)</td>
                <td>N/A</td>
                <td>0</td>
            </tr>
            <tr>
                <td><strong>Dense</strong></td>
                <td>(None, 128)</td>
                <td><strong>ReLU</strong></td>
                <td>100,480</td>
            </tr>
            <tr>
                <td><strong>Dense</strong></td>
                <td>(None, 64)</td>
                <td><strong>ReLU</strong></td>
                <td>8,256</td>
            </tr>
            <tr>
                <td><strong>Dense</strong></td>
                <td>(None, 10)</td>
                <td><strong>Softmax</strong></td>
                <td>650</td>
            </tr>
            <tr>
                <td><strong>Total</strong></td>
                <td></td>
                <td></td>
                <td><strong>109,386</strong></td>
            </tr>
        </tbody>
    </table>
   <h3>Training Configuration</h3>
    <table>
        <thead>
            <tr>
                <th>Parameter</th>
                <th>Value</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Optimizer</strong></td>
                <td><strong>Adam</strong> <span class="citation"></span></td>
            </tr>
            <tr>
                <td><strong>Loss Function</strong></td>
                <td><strong>Categorical Crossentropy</strong> <span class="citation"></span></td>
            </tr>
            <tr>
                <td><strong>Epochs</strong></td>
                <td><strong>10</strong> <span class="citation"></span></td>
            </tr>
            <tr>
                <td><strong>Batch Size</strong></td>
                <td><strong>32</strong> <span class="citation"></span></td>
            </tr>
        </tbody>
    </table>

   <hr>

   <h2>📊 Performance Results</h2>
    
   <p>After 10 epochs of training, the model achieved the following on the validation (test) set:</p>

   <ul>
        <li><strong>Final Validation Accuracy:</strong> <strong>97.08%</strong> (Excellent generalization) <span class="citation"></span></li>
        <li><strong>Validation Loss:</strong> <strong>0.1384</strong> <span class="citation"></span></li>
    </ul>

   <hr>

   <h2>🛠️ Requirements & Setup</h2>
    
   <p>To run this project, you will need the following Python libraries:</p>
    <pre><code>pip install pandas numpy matplotlib scikit-learn tensorflow</code></pre>
    <p>The data files (<code>Train.csv</code>, <code>test.csv</code>, and <code>Train.rar</code>) are required to replicate the training process <span class="citation"></span>.</p>
    <h2>🧑‍💻 How to Run</h2>
    <ol>
        <li>Clone the repository.</li>
        <li>Ensure your data files (like <code>Train.csv</code>) are correctly placed.</li>
        <li>Execute the Jupyter Notebook: <code>handwritten_digit_recognition_using_ANN.ipynb</code> <span class="citation"></span>.</li>
    </ol>
        <hr>
    <em>Made with ❤️ and Keras.</em>

</body>
</html>
