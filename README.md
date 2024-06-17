# X-Ray Görselleri İle Pnömoni Tespiti

Bu proje, göğüs X-ray görüntüleri kullanılarak normal ve pnömoni (akciğer enfeksiyonu) durumlarını sınıflandırmak için derin öğrenme modeli eğitmek amacıyla yapılmıştır. 

Proje, PyTorch kütüphanesi ve RestNet (Residual Neural Network) mimarisi kullanılarak geliştirilmiştir.

## Veri Seti

Veri seti, `chest_xray` klasörü altında aşağıdaki yapıda olmalıdır:

## Dosya yapısı

chest_xray
│

├── test

│ ├── Normal
│ └── PNEUMONIA
│

└── train

├── Normal
└── PNEUMONIA


`train` klasörü, modelin eğitiminde kullanılacak verileri içerirken, `test` klasörü modelin performansını değerlendirmek için kullanılacak verileri içermektedir.

## Kullanım

1. **Gereksinimlerin Kurulumu:**
   - Python 3.x
   - PyTorch
   - torchvision
   - numpy
   - matplotlib
   - seaborn
   - sklearn

## Veri seti

https://www.kaggle.com/datasets/alifrahman/chestxraydataset

Sonuçlar
Eğitim ve değerlendirme sonuçları aşağıdaki adımlarla elde edilmiştir:

Eğitim sonucunda elde edilen en iyi model, test veri seti üzerinde %X doğruluk elde etmiştir.
Karmaşıklık matrisi ve sınıflandırma raporu (precision, recall, F1-score) gibi metrikler kullanılarak modelin performansı değerlendirilmiştir.
