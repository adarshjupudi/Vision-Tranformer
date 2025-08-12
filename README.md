<!DOCTYPE html>
<html>
<head>
<title>Vision Transformer Project</title>
</head>
<body>

  <h1>Vision Transformer (ViT) for CIFAR-10 Classification</h1>
  <p>This repository implements a custom <b>Vision Transformer (ViT)</b> model from scratch using <b>PyTorch</b> for image classification on the <b>CIFAR-10</b> dataset. The project demonstrates the application of transformer architecture to computer vision tasks, utilizing core components like patch embeddings and multi-head self-attention.</p>

  <hr>

  <h2>Files</h2>
  <ul>
    <li><b>Vision Transformer.ipynb:</b> Main Jupyter notebook containing the full implementation, training, and evaluation.</li>
  </ul>

  <hr>

  <h2>Dataset</h2>
  <ul>
    <li><b>CIFAR-10</b> is a standard dataset of 60,000 32x32 color images across 10 classes.</li>
    <li>The dataset is split into 50,000 images for training and 10,000 for testing.</li>
    <li>The data is automatically downloaded using <code>torchvision.datasets.CIFAR10</code>.</li>
  </ul>

  <hr>

  <h2>Architecture</h2>
  <p>The model is built on the Vision Transformer structure, with key components:</p>
  <ul>
    <li><b>Patch Embedding:</b> The input image is split into fixed-size patches, which are flattened and linearly embedded. A learnable class token and positional embeddings are added.</li>
    <li><b>Transformer Encoder:</b> A sequence of transformer encoder layers processes the patch embeddings. Each layer includes a Multi-Head Self-Attention mechanism and a feed-forward network (MLP).</li>
    <li><b>Classification Head:</b> A final classifier uses the class token's output, passed through a linear layer to produce the 10 class predictions.</li>
  </ul>

  <hr>

  <h2>Notebook Workflow</h2>
  <ul>
    <li><b>Data Preparation:</b> Load the CIFAR-10 dataset using <code>torchvision</code>, normalize images, and prepare mini-batches using <code>DataLoader</code>.</li>
    <li><b>Model Construction:</b> Define the <code>PatchEmbedding</code>, <code>MLP</code>, and <code>TransformerEncoderLayer</code> classes, which are then combined to form the complete <code>VisionTransformer</code> model.</li>
    <li><b>Training:</b> The model is trained using <code>CrossEntropyLoss</code> and the <code>Adam</code> optimizer, with accuracy and loss tracked per epoch.</li>
    <li><b>Evaluation:</b> The model's accuracy is measured on the test set.</li>
  </ul>

  <hr>

  <h2>Results</h2>
  <p>The Vision Transformer model achieved a training accuracy of <b>76%</b> and a test accuracy of <b>72%</b> after 10 epochs, demonstrating its ability to learn from the CIFAR-10 dataset.</p>

  <hr>

  <h2>Author</h2>
  <ul>
    <li><b>Author:</b> Adarsh Jupudi</li>
    <li><b>Affiliation:</b> B.Tech Sophomore, Computer Science and Engineering, Indian Institute of Technology Bhubaneswar</li>
    <li><b>LinkedIn:</b> <a href="www.linkedin.com/in/adarsh-jupudi">www.linkedin.com/in/adarsh-jupudi</a></li>
  </ul>

</body>
</html>
