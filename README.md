# VIT_CNN
This project leverages a combination of ViT and CNN models to effectively identify plant illnesses. The ViT model plays a pivotal role in extracting features from plant images. Unlike traditional CNNs, ViT divides an image into small patches and processes them as tokens in a sequence, allowing it to capture global relationships across the image. This feature extraction process provides essential data for further analysis, which aids in identifying specific patterns associated with plant health conditions, making the model highly efficient in recognizing complex features.
The project also incorporates a custom CNN model, which complements the ViT model by focusing on extracting detailed features from the plant leaf image dataset. CNNs are well-known for their ability to capture localized spatial information, such as color, texture, and shape. These characteristics are crucial for diagnosing plant illnesses since certain diseases manifest through specific visual symptoms like spots or discoloration. The CNN thus helps isolate and identify these local features, adding precision to the overall model.
After the ViT and CNN models have extracted features from the plant images, the project utilizes feature concatenation to combine these outputs. By merging the global features from the ViT model with the local features from the CNN, the model benefits from a more comprehensive understanding of the plant images. This combination optimizes the process of plant illness identification, as the fused feature set allows the model to consider broader image patterns and finer details, improving its predictive capabilities.
An Explainable AI (XAI) model is integrated into the system to interpret the predictions made by the ViT and CNN models. While deep learning models often act as "black boxes," XAI techniques such as LIME  ensure transparency by explaining how the model arrives at a particular decision. For instance, they can highlight which specific features (like discolored patches or unusual shapes) contributed most to identifying plant illness. This interpretability not only increases trust in the model but also helps in validating its decisions.
LIME  is an interpretable ML technique that explains the predictions of any black-box model. It works by approximating a complex model locally with a simpler, interpretable model (like linear regression) to explain individual predictions, helping to understand how features influence specific outcomes.
t-SNE (t-distributed Stochastic Neighbor Embedding) is a dimensionality reduction technique for visualizing high-dimensional data. It models similar data points nearby in lower dimensions (typically 2D or 3D) by minimizing divergence between pairwise probabilities. It's widely used for data exploration, especially in clustering.
In conclusion, the concatenation of ViT and CNN features and the interpretability provided by XAI result in a robust and optimized plant illness identification system. The integration of global and local feature analysis improves accuracy. At the same time, the model's explainabilitymodel's explainability ensures that its predictions are precise and reliable, aiding in better decision-making for plant health monitoring.



