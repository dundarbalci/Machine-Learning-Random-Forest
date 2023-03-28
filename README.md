# Machine-Learning-Random-Forest

## Kütüphaneleri İçe Aktarma ve Verileri Yükleme
Sağlanan kod Python dilinde yazılmıştır ve Iris veri kümesi için Random Forest algoritmasının kullanımını gösterir. Gerekli kütüphaneler içe aktarılır, pandas veri kümesini okumak için, numpy matematiksel işlemler için ve görselleştirme için matplotlib kullanılır.
Daha sonra pandas'in read_csv yöntemi kullanılarak Iris veri kümesi içe aktarılır. Beş sütunu vardır, biri bağımlı değişken olmak üzere diğerleri bağımsız değişkenleri temsil eder. Bağımsız değişkenler ölçüm özelliklerini temsil ederken, türler sütunu sınıflandırma için kullanılır.

## Verilerin Eğitilmesi ve Test Setlerine Ayırma
Veri kümesi dört parçaya ayrılır, %67'si eğitim ve %33'ü test için kullanılır. Bu için sklearn.model_selection kütüphanesinden train_test_split yöntemi kullanılır.

## Random Forest Algoritması Modeli Oluşturma
Daha sonra sklearn.ensemble kütüphanesinden Random Forest algoritması içe aktarılır ve bir random forest sınıflandırıcısı nesnesi bir rfc değişkenine atılır. Algoritmada kullanılan karar ağacı sayısı n_estimators parametresiyle belirlenir. Ağaç sayısı ne kadar yüksek olursa, tahmin daha doğru olur.

## Model Performansını Değerlendirme
Model eğitim verisine uyarlandıktan sonra, tahmin yöntemi test verileri üzerinde kullanılarak tahminler yapılır. Sonra sklearn.metrics kütüphanesinden confusion_matrix yöntemi kullanılarak modelin doğruluğu değerlendirilir. Doğruluk, doğru sınıflandırılan örneklerin toplam örneklere oranı olarak hesaplanır.
