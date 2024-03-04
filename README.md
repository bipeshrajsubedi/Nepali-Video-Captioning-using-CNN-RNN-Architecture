### Nepali-Video-Captioning-using-CNN-RNN-Architecture
Descriprtion: Video Captioning using CNN (for image features extraction) and RNN (for language modelling) in Nepali Language. 
The approach involves dataset collection, data preprocessing,
model implementation, and evaluation. By enriching the MSVD
dataset with Nepali captions via Google Translate, the study
trains various CNN-RNN architectures. The research explores the
effectiveness of CNNs (e.g., EfficientNetB0, ResNet101, VGG16)
paired with different RNN decoders like LSTM, GRU, and
BiLSTM. Evaluation involves BLEU and METEOR metrics, with
the best model being EfficientNetB0 + BiLSTM with 1024 hidden
dimensions, achieving a BLEU-4 score of 17 and METEOR score
of 46.

Dataset: MSVD
Original dataset: https://www.cs.utexas.edu/users/ml/clamp/videoDescription/
@InProceedings{chen:acl11,
  title = "Collecting Highly Parallel Data for Paraphrase Evaluation",
  author = "David L. Chen and William B. Dolan",
  booktitle = "Proceedings of the 49th Annual Meeting of the Association for Computational Linguistics (ACL-2011)",
  address = "Portland, OR",
  month = "June",
  year = 2011
}

Nepali dataset (ours): https://www.kaggle.com/datasets/bipeshrajsubedi/msvd-nepali-dataset 

Models Explored:
CNN: ResNet-101, EfficientNetB0, VGG16
RNN: LSTM, GRU, BiLSTM

Findings:
- EfficientNetBO also performed well with LSTM and GRU, surpassing ResNet-101 and VGG16.
- EfficientNetBO + BILSTM with 1024 hidden dimensions outperformed other models.
- Higher METEOR scores suggest that captions effectively convey the main message, even if they vary somewhat from the reference sentences.
- Best model scores: BLEU1: 0.65, BLEU2: 0.41, BLEU3: 0.23, BLEU4: 0.17, METEOR: 0.46

Publication:
This work has been presented in the Proceedings of the International Conference on Technologies for Computer, Electrical, Electronics & Communication (ICT-CEEL 2023), Bhaktapur, Nepal.
Paper link: https://arxiv.org/abs/2311.02699
@article{subedi2023nepali,
  title={Nepali Video Captioning using CNN-RNN Architecture},
  author={Subedi, Bipesh and Singh, Saugat and Bal, Bal Krishna},
  journal={arXiv preprint arXiv:2311.02699},
  year={2023}
}
