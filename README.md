# similarity_embedding_notes
These are the notes or important points which can be helpful in AI 
Common Similarity Metrics
Several metrics can be used to calculate the similarity between two vectors. Here are some of the most common ones:

1. Cosine Similarity
Measures the cosine of the angle between two vectors.
Ranges from -1 (completely dissimilar) to 1 (identical).
Commonly used for text similarity.
Python
import numpy as np

def cosine_similarity(v1, v2):
  return np.dot(v1, v2) / (np.linalg.norm(v1) * np.linalg.norm(v2))
Use code with caution.

2. Euclidean Distance
Measures the straight-line distance between two points in Euclidean space.
Lower values indicate higher similarity.
Often used for image and audio data.
Python
import numpy as np

def euclidean_distance(v1, v2):
  return np.linalg.norm(v1 - v2)
Use code with caution.

3. Manhattan Distance
Measures the distance between two points by summing the absolute differences of their Cartesian coordinates.
Lower values indicate higher similarity.
Often used for text and image data.
Python
import numpy as np

def manhattan_distance(v1, v2):
  return np.sum(np.abs(v1 - v2))
Use code with caution.

Choosing the Right Metric
The best metric depends on the nature of your data and the specific problem you're trying to solve.

Cosine similarity is often preferred when the magnitude of the vectors is less important than the direction.
Euclidean distance is suitable when the magnitude of the differences between the components of the vectors is important.
Manhattan distance is often used as a simpler alternative to Euclidean distance.
