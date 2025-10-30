<h1>The Complete Large Language Model (LLM) Guide</h1>

<p><strong>From Fundamentals to Advanced Implementation</strong></p>

<p>A comprehensive, research-grade resource covering the complete spectrum of Large Language Models - from mathematical foundations to production deployment and ethical considerations.</p>

<div style="background: #f5f5f5; padding: 15px; border-left: 4px solid #007acc; margin: 20px 0;">
<strong>🚀 Quick Start</strong><br>
This guide progresses from fundamental concepts to advanced research frontiers. Each chapter builds upon previous knowledge with practical implementations and mathematical rigor.
</div>

<h2>Table of Contents</h2>
<ul>
  <li><a href="#introduction">1. Introduction to the LLM Revolution</a></li>
  <li><a href="#learning-path">2. Complete Learning Pathway</a></li>
  <li><a href="#mathematical-foundations">3. Mathematical Foundations</a></li>
</ul>

<h2 id="introduction">1. Introduction to the LLM Revolution</h2>

<h3>1.1 What are Large Language Models?</h3>

<p>Large Language Models (LLMs) represent a paradigm shift in artificial intelligence, leveraging deep neural networks with billions to trillions of parameters to understand, generate, and reason with human language.</p>

<p><strong>Core Characteristics:</strong></p>
<ul>
  <li><strong>Scale</strong>: Model sizes ranging from millions to trillions of parameters</li>
  <li><strong>Architecture</strong>: Primarily Transformer-based neural networks</li>
  <li><strong>Training</strong>: Self-supervised learning on massive text corpora</li>
  <li><strong>Emergent Abilities</strong>: Reasoning, code generation, mathematical problem-solving</li>
</ul>

<h3>1.2 Historical Evolution Timeline</h3>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th>Era</th>
    <th>Timeline</th>
    <th>Key Models</th>
    <th>Breakthroughs</th>
  </tr>
  <tr>
    <td><strong>Statistical</strong></td>
    <td>1990-2010</td>
    <td>N-gram models, HMMs</td>
    <td>Probabilistic language modeling</td>
  </tr>
  <tr>
    <td><strong>Neural</strong></td>
    <td>2013-2017</td>
    <td>Word2Vec, LSTM, GRU</td>
    <td>Distributed representations, sequence modeling</td>
  </tr>
  <tr>
    <td><strong>Transformer</strong></td>
    <td>2017-2018</td>
    <td>Original Transformer</td>
    <td>Self-attention mechanism, parallel processing</td>
  </tr>
  <tr>
    <td><strong>Pre-training</strong></td>
    <td>2018-2020</td>
    <td>BERT, GPT-2, RoBERTa</td>
    <td>Transfer learning, bidirectional context</td>
  </tr>
  <tr>
    <td><strong>Large-scale</strong></td>
    <td>2020-2022</td>
    <td>GPT-3, T5, PaLM</td>
    <td>Few-shot learning, scaling laws, reasoning</td>
  </tr>
  <tr>
    <td><strong>Modern</strong></td>
    <td>2022-Present</td>
    <td>GPT-4, Claude, Llama, Mistral</td>
    <td>Multimodality, alignment, open-weight models</td>
  </tr>
</table>

<h3>1.3 Scale Progression Analysis</h3>

<pre><code># Parameter count evolution (2018-2024)
Model Scaling Timeline:
├── ELMo (2018): 94 million parameters
├── BERT-base (2018): 110 million parameters
├── GPT-1 (2018): 117 million parameters
├── GPT-2 (2019): 1.5 billion parameters
├── T5 (2020): 11 billion parameters
├── GPT-3 (2020): 175 billion parameters
├── PaLM (2022): 540 billion parameters
├── GPT-4 (2023): ~1.7 trillion parameters (estimated)
└── Gemini Ultra (2024): ~? trillion parameters
</code></pre>

<h3>1.4 Current Model Landscape</h3>

<p><strong>Major Model Families:</strong></p>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px;">
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>GPT Series (OpenAI)</h4>
    <ul>
      <li>Generative Pre-trained Transformers</li>
      <li>Autoregressive decoder-only architecture</li>
      <li>Strong few-shot learning capabilities</li>
    </ul>
  </div>
  
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>BERT Family (Google)</h4>
    <ul>
      <li>Bidirectional Encoder Representations</li>
      <li>Masked language modeling objective</li>
      <li>Excellent for understanding tasks</li>
    </ul>
  </div>
  
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>T5 Framework (Google)</h4>
    <ul>
      <li>Text-to-Text Transfer Transformer</li>
      <li>Unified framework for all NLP tasks</li>
      <li>Encoder-decoder architecture</li>
    </ul>
  </div>
  
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>Llama Series (Meta)</h4>
    <ul>
      <li>Open-weight foundation models</li>
      <li>Efficient pre-training approaches</li>
      <li>Strong performance per parameter</li>
    </ul>
  </div>
</div>

<h3>1.5 Core Architectural Concepts</h3>

<pre><code>High-Level LLM Architecture:
Input Text → Tokenization → Embedding → Transformer Blocks → Output Head → Generated Text
    │           │             │              │                 │
    │           │             │              └── Multi-Head Attention
    │           │             │                  Layer Normalization
    │           │             │                  Feed-Forward Networks
    │           │             └── Word/Position Embeddings
    │           └── Subword Tokenization (BPE, SentencePiece)
    └── Prompt/Context
</code></pre>

<h2 id="learning-path">2. Complete Learning Pathway</h2>

<h3>2.1 Prerequisite Knowledge Map</h3>

<p><strong>Essential Foundations:</strong></p>

<div style="background: #e8f4f8; padding: 15px; border-radius: 5px;">
<h4>🟦 Beginner Level (Months 1-3)</h4>
<ul>
  <li><strong>Python Programming</strong>: OOP, data structures, libraries</li>
  <li><strong>Linear Algebra</strong>: Vectors, matrices, transformations</li>
  <li><strong>Probability & Statistics</strong>: Distributions, Bayes theorem</li>
  <li><strong>Calculus</strong>: Derivatives, gradients, chain rule</li>
</ul>
</div>

<div style="background: #e8f4f8; padding: 15px; border-radius: 5px; margin-top: 10px;">
<h4>🟩 Intermediate Level (Months 4-6)</h4>
<ul>
  <li><strong>Deep Learning Fundamentals</strong>: Neural networks, backpropagation</li>
  <li><strong>PyTorch/TensorFlow</strong>: Model implementation, training loops</li>
  <li><strong>NLP Basics</strong>: Tokenization, word embeddings, RNNs</li>
  <li><strong>Software Engineering</strong>: Version control, testing, APIs</li>
</ul>
</div>

<div style="background: #e8f4f8; padding: 15px; border-radius: 5px; margin-top: 10px;">
<h4>🟪 Advanced Level (Months 7-12)</h4>
<ul>
  <li><strong>Transformer Architecture</strong>: Self-attention, positional encoding</li>
  <li><strong>Distributed Training</strong>: Data/model parallelism, mixed precision</li>
  <li><strong>Optimization Theory</strong>: Loss landscapes, convergence analysis</li>
  <li><strong>Research Methodology</strong>: Paper reading, experimental design</li>
</ul>
</div>

<h3>2.2 Progressive Learning Roadmap</h3>

<pre><code>Learning Progression (12-Month Plan):
Month 1-2: Mathematical Foundations & Python
Month 3-4: Deep Learning Basics & PyTorch
Month 5-6: NLP Fundamentals & Classical Models
Month 7-8: Transformer Architecture & Implementation
Month 9-10: Pre-training & Fine-tuning Techniques
Month 11-12: Advanced Topics & Research Projects
</code></pre>

<h3>2.3 Practical Project Timeline</h3>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th>Phase</th>
    <th>Projects</th>
    <th>Technologies</th>
    <th>Outcomes</th>
  </tr>
  <tr>
    <td><strong>Beginner</strong></td>
    <td>Text classification, Named Entity Recognition</td>
    <td>scikit-learn, spaCy, BERT</td>
    <td>Basic NLP pipeline understanding</td>
  </tr>
  <tr>
    <td><strong>Intermediate</strong></td>
    <td>Transformer from scratch, Fine-tuning LLMs</td>
    <td>PyTorch, HuggingFace, WandB</td>
    <td>Architecture mastery, training workflows</td>
  </tr>
  <tr>
    <td><strong>Advanced</strong></td>
    <td>Pre-training small LLM, Optimization techniques</td>
    <td>DeepSpeed, FlashAttention, vLLM</td>
    <td>Production-grade model development</td>
  </tr>
</table>

<h2 id="mathematical-foundations">3. Mathematical Foundations</h2>

<h3>3.1 Linear Algebra Essentials</h3>

<p><strong>Vector and Matrix Operations:</strong></p>

<p>Given vectors $x, y \in \mathbb{R}^n$ and matrices $A, B \in \mathbb{R}^{m \times n}$:</p>

<ul>
  <li><strong>Dot Product</strong>: $x \cdot y = \sum_{i=1}^{n} x_i y_i$</li>
  <li><strong>Matrix Multiplication</strong>: $(AB)_{ij} = \sum_{k=1}^{n} A_{ik} B_{kj}$</li>
  <li><strong>Transpose Properties</strong>: $(A^T)_{ij} = A_{ji}$</li>
</ul>

<p><strong>Eigen decomposition:</strong> For square matrix $A$,</p>
<p>$A = Q \Lambda Q^{-1}$ where $\Lambda$ contains eigenvalues and $Q$ contains eigenvectors.</p>

<h3>3.2 Probability Theory</h3>

<p><strong>Key Distributions in LLMs:</strong></p>

<ul>
  <li><strong>Softmax Distribution</strong>: $P(y_i) = \frac{e^{z_i}}{\sum_{j=1}^{K} e^{z_j}}$</li>
  <li><strong>Cross-Entropy Loss</strong>: $L = -\sum_{i=1}^{C} y_i \log(\hat{y}_i)$</li>
  <li><strong>Bayes' Theorem</strong>: $P(A|B) = \frac{P(B|A)P(A)}{P(B)}$</li>
</ul>

<h3>3.3 Information Theory</h3>

<p><strong>Entropy and KL Divergence:</strong></p>

<p><strong>Shannon Entropy</strong>: $H(X) = -\sum_{x \in \mathcal{X}} p(x) \log p(x)$</p>

<p><strong>Cross Entropy</strong>: $H(P, Q) = -\sum_{x \in \mathcal{X}} P(x) \log Q(x)$</p>

<p><strong>KL Divergence</strong>: $D_{KL}(P \| Q) = \sum_{x \in \mathcal{X}} P(x) \log \frac{P(x)}{Q(x)}$</p>

<p><strong>Perplexity</strong>: $\text{PP}(X) = \exp\left(-\frac{1}{N} \sum_{i=1}^{N} \log P(x_i)\right)$</p>

<h3>3.4 Calculus for Optimization</h3>

<p><strong>Gradient Descent Update Rule:</strong></p>

<p>$\theta_{t+1} = \theta_t - \eta \nabla_\theta J(\theta)$</p>

<p>where $\eta$ is learning rate and $J(\theta)$ is the loss function.</p>

<p><strong>Chain Rule for Backpropagation:</strong></p>

<p>$\frac{\partial L}{\partial x} = \frac{\partial L}{\partial y} \cdot \frac{\partial y}{\partial x}$</p>

<h3>3.5 Statistical Learning Theory</h3>

<p><strong>Bias-Variance Decomposition:</strong></p>

<p>$\mathbb{E}[(y - \hat{f}(x))^2] = \text{Bias}[\hat{f}(x)]^2 + \text{Var}[\hat{f}(x)] + \sigma^2$</p>

<p>where:</p>
<ul>
  <li>$\text{Bias}[\hat{f}(x)] = \mathbb{E}[\hat{f}(x)] - f(x)$</li>
  <li>$\text{Var}[\hat{f}(x)] = \mathbb{E}[(\hat{f}(x) - \mathbb{E}[\hat{f}(x)])^2]$</li>
  <li>$\sigma^2$ is irreducible error</li>
</ul>

<h3>3.6 Key Mathematical Theorems</h3>

<p><strong>Central Limit Theorem:</strong></p>
<p>Given i.i.d. random variables $X_1, X_2, ..., X_n$ with mean $\mu$ and variance $\sigma^2$:</p>
<p>$\frac{\bar{X} - \mu}{\sigma/\sqrt{n}} \xrightarrow{d} N(0,1)$ as $n \to \infty$</p>

<p><strong>Law of Large Numbers:</strong></p>
<p>$\bar{X}_n \xrightarrow{a.s.} \mu$ as $n \to \infty$</p>

<h3>3.7 Numerical Linear Algebra</h3>

<p><strong>Singular Value Decomposition (SVD):</strong></p>
<p>$A = U \Sigma V^T$ where:</p>
<ul>
  <li>$U$: left singular vectors (orthogonal)</li>
  <li>$\Sigma$: singular values (diagonal matrix)</li>
  <li>$V$: right singular vectors (orthogonal)</li>
</ul>

<p><strong>Low-Rank Approximation:</strong></p>
<p>$A_k = U_k \Sigma_k V_k^T$ approximates $A$ with rank $k$</p>

<h3>3.8 References & Further Reading</h3>

<ul>
  <li><strong>Linear Algebra</strong>: Gilbert Strang, "Introduction to Linear Algebra"</li>
  <li><strong>Probability</strong>: Sheldon Ross, "A First Course in Probability"</li>
  <li><strong>Information Theory</strong>: Thomas Cover, "Elements of Information Theory"</li>
  <li><strong>Optimization</strong>: Stephen Boyd, "Convex Optimization"</li>
  <li><strong>Deep Learning</strong>: Ian Goodfellow, "Deep Learning"</li>
</ul>

<div style="background: #e8f4f8; padding: 15px; border-radius: 5px; margin-top: 20px;">
<h2 id="programming-fundamentals">4. Programming Fundamentals</h2>

<h3>4.1 Essential Programming Languages</h3>

<p><strong>Core Language Stack for LLM Development:</strong></p>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px;">
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>Python (Primary)</h4>
    <ul>
      <li><strong>Frameworks</strong>: PyTorch, TensorFlow, JAX</li>
      <li><strong>Libraries</strong>: Transformers, NumPy, Pandas</li>
      <li><strong>Use Cases</strong>: Model development, training, research</li>
    </ul>
  </div>
  
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>C++ (Performance)</h4>
    <ul>
      <li><strong>Frameworks</strong>: CUDA, PyTorch C++ API</li>
      <li><strong>Libraries</strong>: Intel MKL, NVIDIA CUDA Toolkit</li>
      <li><strong>Use Cases</strong>: Kernel optimization, inference engines</li>
    </ul>
  </div>
  
  <div style="border: 1px solid #ddd; padding: 15px;">
    <h4>Bash/Shell (DevOps)</h4>
    <ul>
      <li><strong>Tools</strong>: Docker, Kubernetes, Slurm</li>
      <li><strong>Use Cases</strong>: Deployment, cluster management, automation</li>
    </ul>
  </div>
</div>

<h3>4.2 Python Ecosystem Mastery</h3>

<p><strong>Essential Libraries and Their Roles:</strong></p>

<pre><code># Core LLM Development Stack
llm_stack = {
    "deep_learning": ["PyTorch", "TensorFlow", "JAX"],
    "transformer_libs": ["HuggingFace Transformers", "FairSeq", "Megatron-LM"],
    "numerical_computing": ["NumPy", "SciPy", "CuPy"],
    "data_processing": ["Pandas", "PyArrow", "Dask"],
    "experiment_tracking": ["Weights & Biases", "MLflow", "TensorBoard"],
    "distributed_training": ["DeepSpeed", "PyTorch DDP", "Horovod"]
}
</code></pre>

<h3>4.3 PyTorch Fundamentals</h3>

<p><strong>Core Tensor Operations:</strong></p>

<pre><code>import torch
import torch.nn as nn
import torch.nn.functional as F

# Basic tensor operations
x = torch.randn(2, 3)  # 2x3 tensor
y = torch.ones(2, 3)   # 2x3 tensor of ones

# Common operations
z = x + y              # Element-wise addition
z = torch.matmul(x, y.T)  # Matrix multiplication
z = F.softmax(x, dim=-1)  # Softmax activation

# Automatic differentiation
x = torch.tensor(2.0, requires_grad=True)
y = x ** 2
y.backward()  # Compute gradients
print(x.grad)  # dy/dx = 2x = 4.0
</code></pre>

<p><strong>Neural Network Module:</strong></p>

<pre><code>class SimpleNN(nn.Module):
    def __init__(self, input_size, hidden_size, output_size):
        super().__init__()
        self.fc1 = nn.Linear(input_size, hidden_size)
        self.fc2 = nn.Linear(hidden_size, output_size)
        self.dropout = nn.Dropout(0.1)
        
    def forward(self, x):
        x = F.relu(self.fc1(x))
        x = self.dropout(x)
        x = self.fc2(x)
        return x
</code></pre>

<h3>4.4 Distributed Training Fundamentals</h3>

<p><strong>Data Parallelism:</strong></p>

<pre><code>import torch.distributed as dist
from torch.nn.parallel import DistributedDataParallel as DDP

# Initialize distributed training
def setup(rank, world_size):
    dist.init_process_group("nccl", rank=rank, world_size=world_size)
    torch.cuda.set_device(rank)

# Wrap model with DDP
model = SimpleNN(100, 50, 10)
model = DDP(model, device_ids=[rank])
</code></pre>

<p><strong>Mixed Precision Training:</strong></p>

<pre><code>from torch.cuda.amp import autocast, GradScaler

scaler = GradScaler()

for input, target in dataloader:
    optimizer.zero_grad()
    
    with autocast():
        output = model(input)
        loss = criterion(output, target)
    
    scaler.scale(loss).backward()
    scaler.step(optimizer)
    scaler.update()
</code></pre>

<h3>4.5 GPU Programming Basics</h3>

<p><strong>CUDA Fundamentals:</strong></p>

<pre><code># GPU memory management
x = torch.randn(1000, 1000).cuda()  # Move to GPU
y = torch.randn(1000, 1000).cuda()

# GPU operations
z = torch.matmul(x, y)  # Executed on GPU

# Memory statistics
print(torch.cuda.memory_allocated())  # Current memory usage
print(torch.cuda.max_memory_allocated())  # Peak memory usage

# Synchronization
torch.cuda.synchronize()  # Wait for GPU operations to complete
</code></pre>

<h2 id="neural-networks">5. Neural Networks Deep Dive</h2>

<h3>5.1 Biological Inspiration & Mathematical Formulation</h3>

<p><strong>From Biological Neurons to Artificial Neurons:</strong></p>

<p>A single artificial neuron implements:</p>
<p>$y = f\left(\sum_{i=1}^{n} w_i x_i + b\right)$</p>

<p>where:</p>
<ul>
  <li>$x_i$: Input features</li>
  <li>$w_i$: Learnable weights</li>
  <li>$b$: Bias term</li>
  <li>$f$: Activation function</li>
</ul>

<h3>5.2 Activation Functions</h3>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th>Function</th>
    <th>Formula</th>
    <th>Derivative</th>
    <th>Use Cases</th>
  </tr>
  <tr>
    <td><strong>Sigmoid</strong></td>
    <td>$\sigma(x) = \frac{1}{1 + e^{-x}}$</td>
    <td>$\sigma(x)(1 - \sigma(x))$</td>
    <td>Binary classification, gates</td>
  </tr>
  <tr>
    <td><strong>Tanh</strong></td>
    <td>$\tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}$</td>
    <td>$1 - \tanh^2(x)$</td>
    <td>Hidden layers, RNNs</td>
  </tr>
  <tr>
    <td><strong>ReLU</strong></td>
    <td>$\text{ReLU}(x) = \max(0, x)$</td>
    <td>$1$ if $x > 0$, else $0$</td>
    <td>Most hidden layers</td>
  </tr>
  <tr>
    <td><strong>GELU</strong></td>
    <td>$x \Phi(x)$</td>
    <td>Complex</td>
    <td>Transformers, BERT, GPT</td>
  </tr>
  <tr>
    <td><strong>Softmax</strong></td>
    <td>$\frac{e^{x_i}}{\sum_j e^{x_j}}$</td>
    <td>$\text{Softmax}(x_i)(\delta_{ij} - \text{Softmax}(x_j))$</td>
    <td>Output layer, attention</td>
  </tr>
</table>

<h3>5.3 Backpropagation Mathematics</h3>

<p><strong>Chain Rule Formulation:</strong></p>

<p>Given a neural network with loss $L$, the gradient for weight $w_{ij}^{(l)}$ at layer $l$:</p>

<p>$\frac{\partial L}{\partial w_{ij}^{(l)}} = \frac{\partial L}{\partial z_j^{(l)}} \cdot \frac{\partial z_j^{(l)}}{\partial w_{ij}^{(l)}} = \delta_j^{(l)} \cdot a_i^{(l-1)}$</p>

<p>where:</p>
<ul>
  <li>$z_j^{(l)} = \sum_i w_{ij}^{(l)} a_i^{(l-1)} + b_j^{(l)}$ (pre-activation)</li>
  <li>$a_j^{(l)} = f(z_j^{(l)})$ (activation)</li>
  <li>$\delta_j^{(l)} = \frac{\partial L}{\partial z_j^{(l)}}$ (error term)</li>
</ul>

<p><strong>Backward Pass Recursion:</strong></p>

<p>$\delta_j^{(l)} = f'(z_j^{(l)}) \sum_k w_{jk}^{(l+1)} \delta_k^{(l+1)}$</p>

<h3>5.4 Loss Functions</h3>

<p><strong>Common Loss Functions in LLMs:</strong></p>

<p><strong>Cross-Entropy Loss</strong> (Classification):</p>
<p>$L = -\frac{1}{N} \sum_{i=1}^N \sum_{c=1}^C y_{i,c} \log(\hat{y}_{i,c})$</p>

<p><strong>Mean Squared Error</strong> (Regression):</p>
<p>$L = \frac{1}{N} \sum_{i=1}^N (y_i - \hat{y}_i)^2$</p>

<p><strong>Binary Cross-Entropy</strong>:</p>
<p>$L = -\frac{1}{N} \sum_{i=1}^N [y_i \log(\hat{y}_i) + (1-y_i) \log(1-\hat{y}_i)]$</p>

<h3>5.5 Optimization Algorithms</h3>

<p><strong>Stochastic Gradient Descent (SGD):</strong></p>
<p>$\theta_{t+1} = \theta_t - \eta \nabla_\theta J(\theta)$</p>

<p><strong>Momentum SGD:</strong></p>
<p>$v_{t+1} = \gamma v_t + \eta \nabla_\theta J(\theta)$</p>
<p>$\theta_{t+1} = \theta_t - v_{t+1}$</p>

<p><strong>Adam Optimizer:</strong></p>
<p>$m_t = \beta_1 m_{t-1} + (1-\beta_1) g_t$</p>
<p>$v_t = \beta_2 v_{t-1} + (1-\beta_2) g_t^2$</p>
<p>$\hat{m}_t = \frac{m_t}{1-\beta_1^t}$</p>
<p>$\hat{v}_t = \frac{v_t}{1-\beta_2^t}$</p>
<p>$\theta_{t+1} = \theta_t - \eta \frac{\hat{m}_t}{\sqrt{\hat{v}_t} + \epsilon}$</p>

<h3>5.6 Regularization Techniques</h3>

<p><strong>L1/L2 Regularization:</strong></p>
<p>$L_{\text{total}} = L_{\text{data}} + \lambda \sum_i |w_i|$ (L1)</p>
<p>$L_{\text{total}} = L_{\text{data}} + \lambda \sum_i w_i^2$ (L2)</p>

<p><strong>Dropout:</strong></p>
<p>During training: $a_i^{(l)} = \frac{m_i}{1-p} f(z_i^{(l)})$</p>
<p>where $m_i \sim \text{Bernoulli}(1-p)$</p>

<p><strong>Batch Normalization:</strong></p>
<p>$\hat{x}_i = \frac{x_i - \mu_B}{\sqrt{\sigma_B^2 + \epsilon}}$</p>
<p>$y_i = \gamma \hat{x}_i + \beta$</p>

<h3>5.7 Advanced Architectures</h3>

<p><strong>Convolutional Neural Networks (CNNs):</strong></p>
<pre><code>class CNN(nn.Module):
    def __init__(self):
        super().__init__()
        self.conv1 = nn.Conv2d(1, 32, 3, padding=1)
        self.conv2 = nn.Conv2d(32, 64, 3, padding=1)
        self.pool = nn.MaxPool2d(2)
        self.fc = nn.Linear(64 * 7 * 7, 10)
    
    def forward(self, x):
        x = self.pool(F.relu(self.conv1(x)))
        x = self.pool(F.relu(self.conv2(x)))
        x = x.view(-1, 64 * 7 * 7)
        x = self.fc(x)
        return x
</code></pre>

<p><strong>Recurrent Neural Networks (RNNs):</strong></p>
<p>$h_t = \tanh(W_{hh}h_{t-1} + W_{xh}x_t + b_h)$</p>
<p>$y_t = W_{hy}h_t + b_y$</p>

<pre><code>class SimpleRNN(nn.Module):
    def __init__(self, input_size, hidden_size, output_size):
        super().__init__()
        self.hidden_size = hidden_size
        self.i2h = nn.Linear(input_size + hidden_size, hidden_size)
        self.i2o = nn.Linear(input_size + hidden_size, output_size)
    
    def forward(self, input, hidden):
        combined = torch.cat((input, hidden), 1)
        hidden = torch.tanh(self.i2h(combined))
        output = self.i2o(combined)
        return output, hidden
</code></pre>

<h2 id="transformer-architecture">6. Transformer Architecture Mastery</h2>

<h3>6.1 Core Transformer Components</h3>

<p><strong>Complete Transformer Architecture:</strong></p>

<pre><code>Transformer Architecture:
Input → Token Embedding → Positional Encoding → Encoder Stack → Decoder Stack → Output
    │                      │                      │              │
    │                      │                      ├── Multi-Head Self-Attention
    │                      │                      ├── Feed-Forward Network
    │                      │                      ├── Layer Normalization
    │                      │                      └── Residual Connections
    │                      └── sin/cos functions or learned
    └── WordPiece/BPE tokenization
</code></pre>

<h3>6.2 Self-Attention Mechanism</h3>

<p><strong>Scaled Dot-Product Attention:</strong></p>
<p>$\text{Attention}(Q, K, V) = \text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V$</p>

<p>where:</p>
<ul>
  <li>$Q$: Query matrix ($n \times d_k$)</li>
  <li>$K$: Key matrix ($m \times d_k$)</li>
  <li>$V$: Value matrix ($m \times d_v$)</li>
  <li>$d_k$: Dimension of key vectors</li>
</ul>

<p><strong>Multi-Head Attention:</strong></p>
<p>$\text{MultiHead}(Q, K, V) = \text{Concat}(\text{head}_1, ..., \text{head}_h)W^O$</p>
<p>where $\text{head}_i = \text{Attention}(QW_i^Q, KW_i^K, VW_i^V)$</p>

<h3>6.3 Positional Encoding</h3>

<p><strong>Sinusoidal Positional Encoding:</strong></p>
<p>$PE_{(pos, 2i)} = \sin\left(\frac{pos}{10000^{2i/d_{\text{model}}}}\right)$</p>
<p>$PE_{(pos, 2i+1)} = \cos\left(\frac{pos}{10000^{2i/d_{\text{model}}}}\right)$</p>

<p>where:</p>
<ul>
  <li>$pos$: Position in the sequence</li>
  <li>$i$: Dimension index</li>
  <li>$d_{\text{model}}$: Model dimension</li>
</ul>

<h3>6.4 Feed-Forward Networks</h3>

<p><strong>Position-wise Feed-Forward Network:</strong></p>
<p>$\text{FFN}(x) = \max(0, xW_1 + b_1)W_2 + b_2$</p>

<p>In modern transformers, GELU activation is often used:</p>
<p>$\text{GELU}(x) = x \Phi(x)$</p>
<p>where $\Phi(x)$ is the cumulative distribution function of the standard normal distribution.</p>

<h3>6.5 Layer Normalization</h3>

<p><strong>LayerNorm Operation:</strong></p>
<p>$\text{LayerNorm}(x) = \gamma \cdot \frac{x - \mu}{\sqrt{\sigma^2 + \epsilon}} + \beta$</p>

<p>where:</p>
<ul>
  <li>$\mu = \frac{1}{d} \sum_{i=1}^d x_i$</li>
  <li>$\sigma^2 = \frac{1}{d} \sum_{i=1}^d (x_i - \mu)^2$</li>
  <li>$\gamma, \beta$: Learnable parameters</li>
</ul>

<h3>6.6 Complete Transformer Implementation</h3>

<pre><code>import torch
import torch.nn as nn
import math

class MultiHeadAttention(nn.Module):
    def __init__(self, d_model, num_heads):
        super().__init__()
        self.d_model = d_model
        self.num_heads = num_heads
        self.d_k = d_model // num_heads
        
        self.w_q = nn.Linear(d_model, d_model)
        self.w_k = nn.Linear(d_model, d_model)
        self.w_v = nn.Linear(d_model, d_model)
        self.w_o = nn.Linear(d_model, d_model)
        
    def forward(self, q, k, v, mask=None):
        batch_size, seq_len = q.size(0), q.size(1)
        
        # Linear projections and reshape for multi-head
        Q = self.w_q(q).view(batch_size, seq_len, self.num_heads, self.d_k).transpose(1, 2)
        K = self.w_k(k).view(batch_size, seq_len, self.num_heads, self.d_k).transpose(1, 2)
        V = self.w_v(v).view(batch_size, seq_len, self.num_heads, self.d_k).transpose(1, 2)
        
        # Scaled dot-product attention
        scores = torch.matmul(Q, K.transpose(-2, -1)) / math.sqrt(self.d_k)
        
        if mask is not None:
            scores = scores.masked_fill(mask == 0, -1e9)
        
        attn_weights = torch.softmax(scores, dim=-1)
        attn_output = torch.matmul(attn_weights, V)
        
        # Concatenate heads and put through final linear layer
        attn_output = attn_output.transpose(1, 2).contiguous().view(
            batch_size, seq_len, self.d_model
        )
        return self.w_o(attn_output)

class PositionWiseFFN(nn.Module):
    def __init__(self, d_model, d_ff):
        super().__init__()
        self.linear1 = nn.Linear(d_model, d_ff)
        self.linear2 = nn.Linear(d_ff, d_model)
        self.activation = nn.GELU()
        
    def forward(self, x):
        return self.linear2(self.activation(self.linear1(x)))

class TransformerEncoderLayer(nn.Module):
    def __init__(self, d_model, num_heads, d_ff, dropout=0.1):
        super().__init__()
        self.self_attn = MultiHeadAttention(d_model, num_heads)
        self.ffn = PositionWiseFFN(d_model, d_ff)
        self.norm1 = nn.LayerNorm(d_model)
        self.norm2 = nn.LayerNorm(d_model)
        self.dropout = nn.Dropout(dropout)
        
    def forward(self, x, mask=None):
        # Self-attention with residual connection and layer norm
        attn_output = self.self_attn(x, x, x, mask)
        x = self.norm1(x + self.dropout(attn_output))
        
        # Feed-forward with residual connection and layer norm
        ffn_output = self.ffn(x)
        x = self.norm2(x + self.dropout(ffn_output))
        
        return x

class PositionalEncoding(nn.Module):
    def __init__(self, d_model, max_len=5000):
        super().__init__()
        
        pe = torch.zeros(max_len, d_model)
        position = torch.arange(0, max_len, dtype=torch.float).unsqueeze(1)
        div_term = torch.exp(torch.arange(0, d_model, 2).float() * 
                           (-math.log(10000.0) / d_model))
        
        pe[:, 0::2] = torch.sin(position * div_term)
        pe[:, 1::2] = torch.cos(position * div_term)
        pe = pe.unsqueeze(0).transpose(0, 1)
        
        self.register_buffer('pe', pe)
        
    def forward(self, x):
        return x + self.pe[:x.size(0), :]
</code></pre>

<h3>6.7 Encoder-Decoder Architecture</h3>

<p><strong>Cross-Attention Mechanism:</strong></p>
<p>In decoder layers, cross-attention connects encoder outputs to decoder inputs:</p>
<p>$\text{CrossAttention}(Q_{\text{dec}}, K_{\text{enc}}, V_{\text{enc}}) = \text{softmax}\left(\frac{Q_{\text{dec}}K_{\text{enc}}^T}{\sqrt{d_k}}\right)V_{\text{enc}}$</p>

<h3>6.8 Masking Strategies</h3>

<p><strong>Types of Attention Masks:</strong></p>

<pre><code># Causal masking (autoregressive models)
def causal_mask(size):
    mask = torch.triu(torch.ones(size, size), diagonal=1)
    return mask == 0  # Lower triangular matrix

# Padding mask
def padding_mask(input_ids, pad_token_id=0):
    return (input_ids != pad_token_id).unsqueeze(1).unsqueeze(2)

# Combined mask for decoder
def combined_mask(tgt, pad_token_id=0):
    causal_mask = torch.triu(torch.ones(tgt.size(1), tgt.size(1)), diagonal=1)
    padding_mask = (tgt != pad_token_id).unsqueeze(1)
    return padding_mask & (causal_mask == 0)
</code></pre>

<h3>6.9 Modern Variants and Optimizations</h3>

<p><strong>Architectural Improvements:</strong></p>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th>Variant</th>
    <th>Key Innovation</th>
    <th>Use Cases</th>
  </tr>
  <tr>
    <td><strong>ALiBi</strong></td>
    <td>Relative positional encoding without learned parameters</td>
    <td>Long sequence modeling</td>
  </tr>
  <tr>
    <td><strong>RoPE</strong></td>
    <td>Rotary Position Embeddings</td>
    <td>Llama, GPT-NeoX</td>
  </tr>
  <tr>
    <td><strong>FlashAttention</strong></td>
    <td>IO-aware attention algorithm</td>
    <td>Long context, memory efficiency</td>
  </tr>
  <tr>
    <td><strong>SwiGLU</strong></td>
    <td>Gated linear unit activation</td>
    <td>PaLM, Llama 2</td>
  </tr>
  <tr>
    <td><strong>Grouped Query Attention</strong></td>
    <td>Shared key-value heads across query heads</td>
    <td>Llama 2, inference optimization</td>
  </tr>
</table>

<div style="background: #e8f4f8; padding: 15px; border-radius: 5px; margin-top: 20px;">
<h2 id="attention-mechanisms">7. Attention Mechanisms In-Depth</h2>

<h3>7.1 Attention Formalism</h3>

<p><strong>General Attention Formulation:</strong></p>
<p>Given queries $Q$, keys $K$, and values $V$, attention computes:</p>
<p>$\text{Attention}(Q, K, V) = \sum_i \alpha(q, k_i) v_i$</p>
<p>where $\alpha(q, k_i)$ is the attention weight between query $q$ and key $k_i$.</p>

<h3>7.2 Attention Variants</h3>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th>Type</th>
    <th>Formula</th>
    <th>Complexity</th>
    <th>Use Cases</th>
  </tr>
  <tr>
    <td><strong>Full Self-Attention</strong></td>
    <td>$\text{softmax}\left(\frac{QK^T}{\sqrt{d_k}}\right)V$</td>
    <td>$O(n^2 d)$</td>
    <td>Standard transformers, short sequences</td>
  </tr>
  <tr>
    <td><strong>Linear Attention</strong></td>
    <td>$\phi(Q)(\phi(K)^T V)$</td>
    <td>$O(n d^2)$</td>
    <td>Long sequences, memory constraints</td>
  </tr>
  <tr>
    <td><strong>Local Attention</strong></td>
    <td>Window-based computation</td>
    <td>$O(n w d)$</td>
    <td>Images, local dependencies</td>
  </tr>
  <tr>
    <td><strong>Sparse Attention</strong></td>
    <td>Fixed/learned patterns</td>
    <td>$O(n \sqrt{n} d)$</td>
    <td>Very long sequences</td>
  </tr>
  <tr>
    <td><strong>Low-Rank Attention</strong></td>
    <td>Projected attention matrices</td>
    <td>$O(n k d)$</td>
    <td>Approximation, efficiency</td>
  </tr>
</table>

<h3>7.3 Multi-Head Attention Mathematics</h3>

<p><strong>Detailed Multi-Head Formulation:</strong></p>
<p>For head $i$:</p>
<p>$Q_i = Q W_i^Q, \quad K_i = K W_i^K, \quad V_i = V W_i^V$</p>
<p>$\text{head}_i = \text{softmax}\left(\frac{Q_i K_i^T}{\sqrt{d_k}}\right) V_i$</p>
<p>$\text{MultiHead}(Q, K, V) = \text{Concat}(\text{head}_1, ..., \text{head}_h) W^O$</p>

<p><strong>Parameter Count:</strong></p>
<p>Total parameters = $4 \times d_{\text{model}} \times d_{\text{model}}$ (for Q, K, V, O projections)</p>

<h3>7.4 Efficient Attention Mechanisms</h3>

<p><strong>Linformer (Low-Rank Projection):</strong></p>
<p>$K' = E K, \quad V' = F V$ where $E, F \in \mathbb{R}^{k \times n}$</p>
<p>Complexity reduces from $O(n^2)$ to $O(nk)$</p>

<p><strong>Performer (Fast Attention via Orthogonal Random Features):</strong></p>
<p>$\text{Attention}(Q, K, V) \approx \phi(Q) (\phi(K)^T V)$</p>
<p>where $\phi$ is a feature map approximating softmax kernel</p>

<pre><code>class EfficientAttention(nn.Module):
    def __init__(self, d_model, num_heads, feature_dim=256):
        super().__init__()
        self.d_model = d_model
        self.num_heads = num_heads
        self.feature_dim = feature_dim
        
        # Random features for approximation
        self.w = nn.Parameter(torch.randn(feature_dim, d_model // num_heads))
        
    def random_features(self, x):
        # Random feature map for kernel approximation
        x_proj = F.linear(x, self.w)
        return torch.exp(x_proj - x_proj.max(dim=-1, keepdim=True)[0])
    
    def forward(self, q, k, v):
        batch_size, seq_len = q.size(0), q.size(1)
        
        # Apply random feature maps
        q_features = self.random_features(q)
        k_features = self.random_features(k)
        
        # Linear attention computation
        kv_matrix = torch.bmm(k_features.transpose(1,2), v)
        attention_output = torch.bmm(q_features, kv_matrix)
        
        return attention_output
</code></pre>

<h3>7.5 Sparse Attention Patterns</h3>

<p><strong>Fixed Patterns:</strong></p>

<pre><code>def fixed_sparse_attention_mask(seq_len, pattern_type="strided"):
    mask = torch.zeros(seq_len, seq_len)
    
    if pattern_type == "strided":
        # Every other position attends to previous 8 positions
        for i in range(seq_len):
            start = max(0, i - 8)
            mask[i, start:i+1] = 1
            if i % 2 == 0 and i > 0:
                mask[i, i-1] = 1
                
    elif pattern_type == "dilated":
        # Dilated attention pattern
        for i in range(seq_len):
            for j in range(0, i+1, 2):  # Attend to every other position
                if j <= i:
                    mask[i, j] = 1
                    
    return mask.bool()
</code></pre>

<h3>7.6 Long Sequence Attention</h3>

<p><strong>Sliding Window Attention:</strong></p>
<p>Each position only attends to $w$ previous positions:</p>
<p>$\text{Attention}(q_i, K, V) = \sum_{j=\max(0,i-w)}^{i} \alpha(q_i, k_j) v_j$</p>

<p><strong>Block-Sparse Attention:</strong></p>
<pre><code>def block_sparse_attention(q, k, v, block_size=64, num_blocks=4):
    batch_size, seq_len, d_model = q.shape
    
    # Reshape into blocks
    q_blocks = q.view(batch_size, seq_len // block_size, block_size, d_model)
    k_blocks = k.view(batch_size, seq_len // block_size, block_size, d_model)
    v_blocks = v.view(batch_size, seq_len // block_size, block_size, d_model)
    
    output = torch.zeros_like(q)
    
    # Each block attends to previous num_blocks blocks
    for block_idx in range(seq_len // block_size):
        start_block = max(0, block_idx - num_blocks + 1)
        attended_blocks = range(start_block, block_idx + 1)
        
        # Compute attention within attended blocks
        # ... implementation details ...
        
    return output
</code></pre>

<h2 id="training-methodologies">8. Advanced Training Methodologies</h2>

<h3>8.1 Pre-training Objectives</h3>

<p><strong>Autoregressive (Causal) Language Modeling:</strong></p>
<p>$L_{\text{CLM}} = -\sum_{t=1}^T \log P(x_t | x_{&lt;t})$</p>

<p><strong>Masked Language Modeling (BERT-style):</strong></p>
<p>$L_{\text{MLM}} = -\sum_{i \in M} \log P(x_i | x_{\setminus M})$</p>
<p>where $M$ is set of masked positions</p>

<p><strong>Permutation Language Modeling (XLNet):</strong></p>
<p>$L_{\text{PLM}} = \mathbb{E}_{z \sim Z_T} \left[ \sum_{t=1}^T \log P(x_{z_t} | x_{z_{&lt;t}}) \right]$</p>

<h3>8.2 Scaling Laws</h3>

<p><strong>Kaplan Scaling Laws:</strong></p>
<p>$L(N, D) = \left(\frac{N_c}{N}\right)^{\alpha_N} + \left(\frac{D_c}{D}\right)^{\alpha_D} + L_\infty$</p>

<p>where:</p>
<ul>
  <li>$N$: Model parameters</li>
  <li>$D$: Training tokens</li>
  <li>$N_c, D_c$: Critical values</li>
  <li>$\alpha_N, \alpha_D$: Scaling exponents</li>
  <li>$L_\infty$: Irreducible loss</li>
</ul>

<p><strong>Chinchilla Optimal Scaling:</strong></p>
<p>For compute budget $C$, optimal model size $N$ and tokens $D$ satisfy:</p>
<p>$N \propto C^{0.5}, \quad D \propto C^{0.5}$</p>

<h3>8.3 Distributed Training Strategies</h3>

<p><strong>Data Parallelism:</strong></p>
<pre><code># PyTorch DDP Example
import torch.distributed as dist
from torch.nn.parallel import DistributedDataParallel as DDP

def train_ddp(rank, world_size):
    # Initialize process group
    dist.init_process_group("nccl", rank=rank, world_size=world_size)
    
    # Model and data
    model = TransformerModel().to(rank)
    ddp_model = DDP(model, device_ids=[rank])
    
    # Training loop
    for batch in dataloader:
        loss = ddp_model(batch)
        loss.backward()
        optimizer.step()
</code></pre>

<p><strong>Model Parallelism:</strong></p>
<pre><code>class ModelParallelTransformer(nn.Module):
    def __init__(self, num_devices):
        super().__init__()
        self.num_devices = num_devices
        self.layers = nn.ModuleList([
            TransformerLayer().to(f"cuda:{i % num_devices}")
            for i in range(num_layers)
        ])
    
    def forward(self, x):
        for i, layer in enumerate(self.layers):
            device = f"cuda:{i % self.num_devices}"
            x = x.to(device)
            x = layer(x)
        return x
</code></pre>

<p><strong>Pipeline Parallelism:</strong></p>
<pre><code>from torch.distributed.pipeline.sync import Pipe

# Split model across devices
model = LargeTransformer()
model_parts = split_model_into_partitions(model, num_partitions=4)

# Create pipeline
model_pipe = Pipe(model_parts, chunks=8)  # Micro-batches

# Training
output = model_pipe(input)
loss = criterion(output, target)
loss.backward()
</code></pre>

<h3>8.4 Mixed Precision Training</h3>

<p><strong>FP16/FP32 Mixed Precision:</strong></p>
<pre><code>from torch.cuda.amp import autocast, GradScaler

scaler = GradScaler()

for input, target in dataloader:
    optimizer.zero_grad()
    
    with autocast():
        output = model(input)
        loss = criterion(output, target)
    
    scaler.scale(loss).backward()
    scaler.step(optimizer)
    scaler.update()
</code></pre>

<p><strong>BF16 Support:</strong></p>
<pre><code># BF16 has better dynamic range than FP16
torch.set_float32_matmul_precision('medium')  # Use TF32 for matmuls

model = model.to(torch.bfloat16)
for input, target in dataloader:
    input = input.to(torch.bfloat16)
    output = model(input)
    # No need for gradient scaling with BF16
</code></pre>

<h3>8.5 Optimization Techniques</h3>

<p><strong>AdamW Optimizer:</strong></p>
<p>$\theta_{t+1} = \theta_t - \eta \left( \frac{\hat{m}_t}{\sqrt{\hat{v}_t} + \epsilon} + \lambda \theta_t \right)$</p>

<p><strong>Learning Rate Schedules:</strong></p>

<p><strong>Linear Warmup + Cosine Decay:</strong></p>
<pre><code>def get_cosine_schedule_with_warmup(optimizer, num_warmup_steps, num_training_steps):
    def lr_lambda(current_step):
        if current_step < num_warmup_steps:
            return float(current_step) / float(max(1, num_warmup_steps))
        progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
        return max(0.0, 0.5 * (1.0 + math.cos(math.pi * progress)))
    
    return torch.optim.lr_scheduler.LambdaLR(optimizer, lr_lambda)
</code></pre>

<h3>8.6 Regularization Methods</h3>

<p><strong>Weight Decay:</strong></p>
<p>$L_{\text{total}} = L_{\text{task}} + \lambda \sum \theta^2$</p>

<p><strong>Gradient Clipping:</strong></p>
<pre><code># Global gradient clipping
torch.nn.utils.clip_grad_norm_(model.parameters(), max_norm=1.0)

# Per-parameter clipping
for param in model.parameters():
    if param.grad is not None:
        param.grad.data.clamp_(-1.0, 1.0)
</code></pre>

<p><strong>Stochastic Depth:</strong></p>
<pre><code>class StochasticDepth(nn.Module):
    def __init__(self, drop_prob):
        super().__init__()
        self.drop_prob = drop_prob
    
    def forward(self, x, layer):
        if self.training and torch.rand(1) < self.drop_prob:
            return x  # Skip layer
        return layer(x)
</code></pre>

<h2 id="fine-tuning-techniques">9. Fine-tuning and Adaptation</h2>

<h3>9.1 Full Fine-tuning</h3>

<p><strong>Standard Fine-tuning Process:</strong></p>
<pre><code>def full_finetune(model, train_dataloader, num_epochs=3):
    optimizer = AdamW(model.parameters(), lr=5e-5)
    
    for epoch in range(num_epochs):
        model.train()
        for batch in train_dataloader:
            outputs = model(**batch)
            loss = outputs.loss
            loss.backward()
            optimizer.step()
            optimizer.zero_grad()
</code></pre>

<h3>9.2 Parameter-Efficient Fine-tuning (PEFT)</h3>

<h4>9.2.1 LoRA (Low-Rank Adaptation)</h4>

<p><strong>LoRA Mathematical Formulation:</strong></p>
<p>$W' = W + \Delta W = W + BA$</p>
<p>where $B \in \mathbb{R}^{d \times r}$, $A \in \mathbb{R}^{r \times k}$, $r \ll \min(d,k)$</p>

<pre><code>class LoRALayer(nn.Module):
    def __init__(self, base_layer, rank=8, alpha=16):
        super().__init__()
        self.base_layer = base_layer
        self.rank = rank
        self.alpha = alpha
        
        # LoRA matrices
        self.lora_A = nn.Parameter(torch.randn(base_layer.in_features, rank))
        self.lora_B = nn.Parameter(torch.zeros(rank, base_layer.out_features))
        
    def forward(self, x):
        base_output = self.base_layer(x)
        lora_output = x @ self.lora_A @ self.lora_B
        return base_output + (self.alpha / self.rank) * lora_output

def apply_lora_to_linear_layers(model, rank=8):
    for name, module in model.named_children():
        if isinstance(module, nn.Linear):
            # Replace with LoRA layer
            setattr(model, name, LoRALayer(module, rank=rank))
        else:
            apply_lora_to_linear_layers(module, rank)
</code></pre>

<h4>9.2.2 Adapter Layers</h4>

<pre><code>class Adapter(nn.Module):
    def __init__(self, dim, adapter_dim=64):
        super().__init__()
        self.down_proj = nn.Linear(dim, adapter_dim)
        self.up_proj = nn.Linear(adapter_dim, dim)
        self.activation = nn.GELU()
        
    def forward(self, x):
        return x + self.up_proj(self.activation(self.down_proj(x)))

class TransformerWithAdapters(nn.Module):
    def __init__(self, base_transformer):
        super().__init__()
        self.base = base_transformer
        
        # Add adapters after attention and FFN
        for layer in self.base.layers:
            layer.attention_adapter = Adapter(layer.self_attn.d_model)
            layer.ffn_adapter = Adapter(layer.ffn.d_model)
    
    def forward(self, x):
        for layer in self.base.layers:
            # Original attention
            attn_output = layer.self_attn(x)
            x = layer.attention_adapter(attn_output)
            
            # Original FFN
            ffn_output = layer.ffn(x)
            x = layer.ffn_adapter(ffn_output)
        
        return x
</code></pre>

<h3>9.3 Prompt-based Methods</h3>

<h4>9.3.1 Prompt Tuning</h4>

<pre><code>class PromptTuning(nn.Module):
    def __init__(self, model, prompt_length=20):
        super().__init__()
        self.model = model
        self.prompt_length = prompt_length
        self.prompt_embeddings = nn.Parameter(
            torch.randn(prompt_length, model.config.hidden_size)
        )
        
    def forward(self, input_ids, attention_mask=None):
        batch_size = input_ids.shape[0]
        
        # Get original embeddings
        inputs_embeds = self.model.get_input_embeddings()(input_ids)
        
        # Concatenate prompt embeddings
        prompt_embeds = self.prompt_embeddings.unsqueeze(0).repeat(batch_size, 1, 1)
        inputs_embeds = torch.cat([prompt_embeds, inputs_embeds], dim=1)
        
        # Adjust attention mask
        if attention_mask is not None:
            prompt_mask = torch.ones(batch_size, self.prompt_length).to(attention_mask.device)
            attention_mask = torch.cat([prompt_mask, attention_mask], dim=1)
        
        return self.model(inputs_embeds=inputs_embeds, attention_mask=attention_mask)
</code></pre>

<h4>9.3.2 P-Tuning</h4>

<pre><code>class PTuning(nn.Module):
    def __init__(self, model, prompt_length=20, prompt_hidden_size=512):
        super().__init__()
        self.model = model
        self.prompt_length = prompt_length
        
        # LSTM for prompt generation
        self.lstm = nn.LSTM(
            input_size=model.config.hidden_size,
            hidden_size=prompt_hidden_size,
            num_layers=2,
            bidirectional=True,
            batch_first=True
        )
        
        self.mlp = nn.Sequential(
            nn.Linear(2 * prompt_hidden_size, model.config.hidden_size),
            nn.ReLU(),
            nn.Linear(model.config.hidden_size, model.config.hidden_size)
        )
        
    def forward(self, input_ids, attention_mask=None):
        batch_size = input_ids.shape[0]
        
        # Generate continuous prompts
        prompt_tokens = torch.arange(self.prompt_length).unsqueeze(0).repeat(batch_size, 1)
        prompt_embeds = self.model.get_input_embeddings()(prompt_tokens)
        
        # Process through LSTM and MLP
        lstm_out, _ = self.lstm(prompt_embeds)
        continuous_prompts = self.mlp(lstm_out)
        
        # Get original embeddings and concatenate
        inputs_embeds = self.model.get_input_embeddings()(input_ids)
        inputs_embeds = torch.cat([continuous_prompts, inputs_embeds], dim=1)
        
        # Adjust attention mask
        if attention_mask is not None:
            prompt_mask = torch.ones(batch_size, self.prompt_length).to(attention_mask.device)
            attention_mask = torch.cat([prompt_mask, attention_mask], dim=1)
        
        return self.model(inputs_embeds=inputs_embeds, attention_mask=attention_mask)
</code></pre>

<h3>9.4 Instruction Tuning</h3>

<p><strong>Instruction Format:</strong></p>
<pre><code>instruction_prompt = """
Below is an instruction that describes a task. Write a response that appropriately completes the request.

### Instruction:
{instruction}

### Response:
"""
</code></pre>

<p><strong>Supervised Fine-tuning (SFT):</strong></p>
<pre><code>def instruction_tuning_loss(model, batch):
    """Compute loss for instruction following"""
    instructions = batch["instruction"]
    responses = batch["response"]
    
    # Format input with instruction template
    formatted_inputs = [
        f"Instruction: {inst}\n\nResponse: {resp}"
        for inst, resp in zip(instructions, responses)
    ]
    
    # Tokenize and compute loss
    inputs = tokenizer(formatted_inputs, return_tensors="pt", padding=True, truncation=True)
    outputs = model(**inputs, labels=inputs["input_ids"])
    
    return outputs.loss
</code></pre>

<h3>9.5 Reinforcement Learning from Human Feedback (RLHF)</h3>

<p><strong>Three-Stage RLHF Process:</strong></p>

<pre><code># Stage 1: Supervised Fine-tuning
sft_trainer = SFTTrainer(
    model=base_model,
    train_dataset=instruction_data,
    formatting_func=format_instruction
)

# Stage 2: Reward Model Training
class RewardModel(nn.Module):
    def __init__(self, base_model):
        super().__init__()
        self.transformer = base_model
        self.value_head = nn.Linear(base_model.config.hidden_size, 1)
    
    def forward(self, input_ids, attention_mask):
        outputs = self.transformer(input_ids, attention_mask=attention_mask)
        last_hidden_state = outputs.last_hidden_state
        # Use the EOS token for reward prediction
        eos_token_hidden = last_hidden_state[:, -1, :]
        reward = self.value_head(eos_token_hidden)
        return reward

# Stage 3: PPO Training
def ppo_training_step(policy_model, reward_model, prompts):
    # Generate responses with current policy
    with torch.no_grad():
        old_responses = policy_model.generate(prompts)
        old_rewards = reward_model(old_responses)
    
    # Update policy using PPO
    # ... PPO implementation details ...
</code></pre>

<h3>9.6 Evaluation Metrics for Fine-tuning</h3>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr style="background-color: #f2f2f2;">
    <th>Metric</th>
    <th>Formula</th>
    <th>Interpretation</th>
  </tr>
  <tr>
    <td><strong>Perplexity</strong></td>
    <td>$\exp\left(-\frac{1}{N}\sum_{i=1}^N \log P(w_i|w_{&lt;i})\right)$</td>
    <td>Lower is better</td>
  </tr>
  <tr>
    <td><strong>BLEU Score</strong></td>
    <td>BP $\cdot$ $\exp\left(\sum_{n=1}^N w_n \log p_n\right)$</td>
    <td>0-100, higher better</td>
  </tr>
  <tr>
    <td><strong>ROUGE Score</strong></td>
    <td>$\frac{\text{Overlap}}{\text{Reference Length}}$</td>
    <td>Recall-oriented</td>
  </tr>
  <tr>
    <td><strong>Accuracy</strong></td>
    <td>$\frac{\text{Correct}}{\text{Total}}$</td>
    <td>Classification tasks</td>
  </tr>
</table>

<div style="background: #e8f4f8; padding: 15px; border-radius: 5px; margin-top: 20px;">
<h4>📚 Next Chapters Preview</h4>
<p><strong>Chapter 10</strong>: Inference Optimization (quantization, pruning, speculative decoding)<br>
<strong>Chapter 11</strong>: Comprehensive Evaluation (benchmarks, safety, robustness)<br>
<strong>Chapter 12</strong>: Production Deployment (serving, monitoring, scaling)</p>
</div>
</html>
