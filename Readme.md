## Linux Ağ Yönetimi Projesi

Kişisel Bilgisayarınızda Virtualbox üzerinde; 

<code>İsterler</code>

* Ubuntu Desktop 18 veya 20 yükleyin. 
* Hostname-bilgisayar ismini uPC1 olarak isimlendirin. Kullanıcı adı olarak soyadınızı seçin.
* TinyCore Linux (DCore Linux) Yükleyin. hostname-bilgisayar ismini DC1 olarak isimlendirin. Kullanıcı adı olarak isminizi seçin. 
* Ubuntu 18 veya 20 Server yükleyin. hostname-bilgisayar ismini userver1 olarak isimlendirin. Kullanıcı adı olarak soyadınızı seçin.
* Birbirine bağlantılı Klonlama (Çoğalt) yaparak her birisinden iki tane daha klon üretin.

Klonladıktan sonra bilgisayarların isimlerini uPC2,uPC3, DC2, DC3, userver2, userver3 olarak değiştirin.

<h4>Senaryo 1</h4> 
<code>Senaryo 1.1</code>

* Ubuntu Desktop için Ağ bağdaştırıcı ayarlarını NAT olarak ayarlayıp HOST (Kullandığınız) bilgisayardan SSH bağlantısı yapabildiğinizi (PORT yönlendirme ayarlarını yaptıktan sonra), ping yapamadığınızı gösterin. 

<code>Dosya Gönderimi</code>
* HOST bilgisayardaki dosya ismi soyadiniz.txt şeklinde olan bir dosyayı misafir (guest) işletim sistemine Misafir eklentileri yükledikten sonra kopyala yapıştır yaparak gerçekleştiriniz.

<code>Senaryo 1.2</code>
* Dcore işletim sisteminin ağ bağdaştırıcı ayarlarını Köprü bağdaştırıcı olarak seçtikten sonra DC1 IP adresini bulun. SSH bağlantısı yapabilmeniz için gerekli yüklemeleri yaptıktan sonra HOST (Kullandığınız) bilgisayardan SSH bağlantısı ve ping yapamadığınızı gösterin. 

<code>Senaryo 1.3</code>
* Ubuntu Server için yanlızca anamakine bağdaştırıcısı olarak ayarlama yaptıktan sonra IP adresini bulun. SSH bağlantısı yapabilmeniz için gerekli yüklemeleri yaptıktan sonra HOST (Kullandığınız) bilgisayardan SSH bağlantısı ve ping yapamadığınızı gösterin. 

</br>

<h4>Senaryo 2 </h4>

    Numaranızın son iki rakamı S ve R olarak kabul edilmiştir. 

<code>Senaryo 2.1</code>
* userver1, userver2 ve userver3 için ağ bağdaştırıcı ayarlarını dahili ağ olarak ayarlayın. Bilgisayarların IP adreslerini statik olarak aşağıda verilen şekilde ayarlayın : 

<ins> userver1:</ins> 192.168.R.S

<ins>userver2:</ins> 192.168.R.S+1

<ins>userver3:</ins> 192.168.R.S+2

<code>Senaryo 2.2</code>
* Bu üç bilgisayardan birbirilerine ssh yapabildiğinizi ama HOST bilgisayardan bunlara SSH yapamadığınızı gösterin.  ping komutunu kullanarak bu bilgisayarlar arasında haberleşmelerin olduğunu gösterin.

<code>Senaryo 2.3</code>
* userver1 bilgisayardaki dosya ismi adiniz.txt, soyadiniz.txt ve numaraniz.txt şeklinde olan bir dosyaları userver2 bilgisayarına gönderiniz. Gönderim işlemi için sFTP veya SCP protokolünü kullanmanız gerekir.

</br>

<h4>Senaryo 3</h4> 

* uPC1 , uPC2 , userver1 ve userver2 için bir ağ bağdaştırıcısını NAT, diğerini dahili ağ olarak ayarlayın.

   * uPC1 ve userver1 dahili ağ ismini dahili1, 

   * uPC2 ve userver2 dahili ağ ismini dahili2 olarak ayarlayın.

    * userver1 ve userver2 için üçüncü bir ağ bağdaştırıcısını yine dahili3 olarak dahili ağ olarak ayarlayın.

<i>uPC1 üzerinden veri paketlerinin userver1, userver2 ve uPC2 bilgisayarlarına ayrı ayrı nasıl gittiğini gösteriniz. Bunun için uygun bir komut kullanmanızı gerekiyor.</i>

   



<h5><code>Kazanımlar</code></h5>

*  Router nedir ve nasıl kullanılır ?</br>
*  SSH bağlantısı nedir ve nasıl yapılır ?
*  IP sorgulama 
*  Static IP ayarlama
*  Ubuntuda Network ağ yapısı
*  Dcore nedir ve nasıl kullanılır ?
*  Sanal makineleri klonlama 
*  Ağ bağlantı türleri ve özellikleri
*  Host makineden sanal makineye veri gönderimi
*  Sanal makinelerin birbiri ile haberleşmesi
*  Veri gönderirken ağ takibi
*  Quagga nedir ?

[<img src="https://hayalindekiyasam.files.wordpress.com/2020/07/oldu2.png">](https://github.com/melikeoguz/Ubuntu/blob/master/170201028%20Melike%20Oğuz.pdf)


