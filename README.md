We have applied a crystal graph convolutional neural network to conduct a high-throughput screening of most possible recipe for the HOIP candidate and by investigating the property of HOIP materials. The work has been adapted from the paper ["Crystal Graph Convolutional Neural Networks for an Accurate and Interpretable Prediction of Material Properties"](https://arxiv.org/abs/1710.10324), and its code that can be found on [GitHub](https://github.com/txie-93/cgcnn). We use the model to predict band-gap properties for HOIP crystals that were obtained from [this](https://www.nature.com/articles/sdata201757) HOIP dataset. The original model has been adapted to the following tasks:

- Predict band-gap values using pre-trained CGCNN (found in original repository)
- Train CGCNN model from scratch using only HOIP data
- Apply transfer learning, using pre-trained model and HOIP data
- Test the performance of a different loss function

Please download and extract the tarball provided from the dataset source. Use the hoip_band_gap.csv(renamed to id_prop.csv) and atom_init.json file by moving it into the folder with all the cif files.
