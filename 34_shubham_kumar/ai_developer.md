# AI Developer Interview Questions (One-Line Answers)

## Python for AI

1. Why is Python preferred for AI? 
  — It is simple, fast to prototype, and has strong AI libraries.

2. What are generators? 
  — They yield items one at a time and save memory in large data pipelines.

3. List vs NumPy array? 
  — Lists are flexible and slow; NumPy arrays are fast and memory-efficient for math.

4. What is a decorator? 
  — A decorator modifies a function without changing its core logic.

5. What is the GIL? 
  — It limits Python threads from running true parallel CPU code in CPython.

6. Multiprocessing vs multithreading? 
  — Threads share memory and suit I/O; processes use separate memory and suit CPU tasks.

7. What is vectorization? 
  — It uses array operations to avoid slow Python loops.

8. How does Python manage memory? 
  — It uses reference counting and garbage collection.

9. Which Python libraries are common in AI? 
  — NumPy, Pandas, PyTorch, TensorFlow, Scikit-learn, and Hugging Face.

## Math for ML

10. What is gradient descent? 
  — It updates weights step by step to reduce loss.

11. Why are derivatives important? 
  — They show how changing a parameter affects the loss.

12. What is a convex function? 
  — A function where any local minimum is also a global minimum.

13. Why normalize data? 
  — It makes training faster and more stable.

14. L1 vs L2 regularization? 
  — L1 adds sparsity; L2 shrinks weights smoothly.

15. What are eigenvalues and eigenvectors? 
  — They describe directions and scaling in matrix transformations.

16. What is SVD? 
  — It factorizes matrices for dimensionality reduction and recommendation systems.

17. Probability vs likelihood? 
  — Probability is about data given parameters; likelihood is about parameters given data.

18. What is Bayes theorem? 
  — It updates belief using new evidence.

19. What is bias-variance tradeoff? 
  — It balances underfitting and overfitting.

## ML Basics

20. AI vs ML vs Deep Learning? 
  — AI is broad, ML learns from data, and deep learning uses neural networks.

21. Supervised vs unsupervised learning? 
  — Supervised uses labels; unsupervised finds patterns without labels.

22. What is reinforcement learning? 
  — An agent learns by taking actions and receiving rewards.

23. Classification vs regression? 
  — Classification predicts labels; regression predicts numbers.

24. What is overfitting? 
  — The model memorizes training data and fails to generalize.

25. What is underfitting? 
  — The model is too simple to learn the pattern.

26. How do you prevent overfitting? 
  — Use more data, regularization, early stopping, and simpler models.

27. What is cross-validation? 
  — It tests a model on multiple folds to reduce evaluation bias.

28. What is a train-validation-test split? 
  — It separates training, tuning, and final evaluation.

29. What is feature engineering? 
  — It creates useful inputs from raw data.

30. Feature selection vs feature extraction? 
  — Selection keeps existing features; extraction creates new ones.

31. What are hyperparameters? 
  — They control training behavior and are set before training.

32. What is a Random Forest? 
  — It combines many decision trees to improve accuracy and stability.

33. What is a Decision Tree? 
  — It splits data using feature-based rules to make predictions.

34. What is XGBoost? 
  — It is a fast, powerful gradient boosting algorithm.

35. What is KNN? 
  — It predicts using the nearest labeled examples.

36. What is SVM? 
  — It finds a boundary that maximizes the margin between classes.

37. What is Naive Bayes? 
  — It is a fast probabilistic classifier based on Bayes theorem.

38. What is PCA? 
  — It reduces features while keeping most useful variance.

39. What is K-Means? 
  — It groups data by minimizing distances to cluster centers.

## Metrics

40. Accuracy vs precision? 
  — Accuracy measures all correct predictions; precision measures correctness of positive predictions.

41. Precision vs recall? 
  — Precision reduces false positives; recall reduces false negatives.

42. What is the F1 score? 
  — It balances precision and recall.

43. What is a confusion matrix? 
  — It summarizes TP, TN, FP, and FN outcomes.

44. What is ROC-AUC? 
  — It measures how well a classifier ranks positives above negatives.

45. What is MSE? 
  — It penalizes larger errors heavily.

46. What is MAE? 
  — It measures average absolute prediction error.

47. What is R²? 
  — It shows how much variance the model explains.

48. When is accuracy a bad metric? 
  — When classes are highly imbalanced.

## Deep Learning

49. What is a neural network? 
  — It learns patterns through layers of connected neurons.

50. What is a perceptron? 
  — It is a single neuron that makes a simple linear decision.

51. What is backpropagation? 
  — It propagates error backward to update model weights.

52. What is an activation function? 
  — It adds non-linearity so networks can learn complex patterns.

53. Why is ReLU popular? 
  — It is simple, fast, and helps deep networks train better.

54. What is dropout? 
  — It randomly disables neurons to reduce overfitting.

55. What is batch normalization? 
  — It stabilizes training by normalizing layer outputs.

56. Batch gradient vs mini-batch gradient? 
  — Batch uses full data; mini-batch uses smaller chunks for speed.

57. What is an epoch? 
  — One full pass over the training data.

58. What is batch size? 
  — It is the number of samples used per update.

59. CNN vs RNN? 
  — CNNs are for spatial data; RNNs are for sequential data.

60. What is transfer learning? 
  — It fine-tunes a pre-trained model for a new task.

61. What is ResNet? 
  — It uses skip connections to train very deep networks.

62. What is attention? 
  — It lets a model focus on the most relevant parts of input.

## Computer Vision

63. What is a CNN architecture? 
  — It stacks convolution, activation, pooling, and dense layers.

64. Why use convolution instead of fully connected layers? 
  — It saves parameters and preserves spatial structure.

65. What is padding? 
  — It preserves border information during convolution.

66. What is stride? 
  — It controls how much the filter moves each step.

67. What is object detection? 
  — It finds both what objects are and where they are.

68. YOLO vs Faster R-CNN? 
  — YOLO is faster; Faster R-CNN is usually more accurate.

69. What is image augmentation? 
  — It creates new training samples by transforming images.

## NLP and LLMs

70. What is NLP? 
  — It helps machines understand and generate human language.

71. What is tokenization? 
  — It splits text into smaller tokens for model input.

72. What are embeddings? 
  — They turn words or documents into dense vectors.

73. TF-IDF vs Word2Vec? 
  — TF-IDF is frequency-based; Word2Vec learns semantic meaning.

74. What is BERT? 
  — It is a bidirectional transformer encoder for language understanding.

75. What is GPT? 
  — It is a decoder-based model for text generation.

76. What are transformers? 
  — They use attention instead of recurrence for sequence modeling.

77. What is self-attention? 
  — It lets each token relate to every other token in context.

78. What is positional encoding? 
  — It gives transformers information about token order.

79. What is prompt engineering? 
  — It designs inputs that guide model behavior.

80. What is RAG? 
  — It combines retrieval with generation for grounded responses.

81. What are vector databases? 
  — They store embeddings for fast similarity search.

82. What is hallucination? 
  — It is when the model generates plausible but false information.

## MLOps and Deployment

83. How do you deploy an ML model? 
  — Wrap it in an API, containerize it, and deploy it to a server or cloud.

84. Why use FastAPI for AI? 
  — It is fast, async-friendly, and easy to document.

85. What is model versioning? 
  — It tracks models, data, and experiments over time.

86. What is Docker for ML? 
  — It packages code and dependencies into a portable container.

87. What is model drift? 
  — It is when model performance degrades because the data changes.

88. What is CI/CD for ML? 
  — It automates testing, training, and deployment of ML systems.

## Practical AI

89. How do you design a chatbot? 
  — Use an LLM, RAG, memory, and an API layer.

90. How do you build an image classification API? 
  — Serve a model through FastAPI or Triton with GPU support.

91. How do you build a recommendation system? 
  — Retrieve candidates first, then rank them with a scoring model.

92. What is LoRA? 
  — It fine-tunes LLMs efficiently by training only small adapter matrices.

93. What is fine-tuning? 
  — It updates model weights for a specific task.

94. What is a context window? 
  — It is the maximum amount of text an LLM can process at once.

95. What is quantization? 
  — It reduces model size and memory use by lowering precision.

96. What is tool calling in LLMs? 
  — It lets the model trigger external tools or APIs.

97. What is prompt injection? 
  — It is a security attack that manipulates model instructions.

98. What is agentic AI? 
  — It uses planning and tool use to complete multi-step tasks.

99. What are multi-agent systems? 
  — They use several specialists working together on one problem.

100. What is MCP? 
  — It is a protocol for connecting AI systems to tools and data sources.
