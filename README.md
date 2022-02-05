<h1>AngularJS Hakkında Her Şey</h1>
<ul>
  <li>AngularJS, HTML'yi yeni niteliklerle genişletir. </li>
  <li>AngularJS, tek sayfa uygulamaları (SPA= > Single Page Application) için mükemmeldir. </li>
  <li>Google tarafından geliştirilmiştir ve desteklenmektedir. </li>
  <li>AngularJS ile bir sayfa içerisinde olaylar yönetilebilmektedir. Url değişir ancak sayfa reflesh olmaz. </li>
  <li>Tamamen tarayıcıda çalışan javascript uygulamasıdır. Bir javascript kütüphanesidir. </li>
  <li>Tamamen bir frontend tarafından değerlendirilen bir yapıdır. </li>
  <li>API: Bir bir data mı bir veri tabanına mı ihtiyaç var? Buna göre bir API kullanımı yapmamız gerekir. Örneğin bir film sitesinde veri çekme veya banka sitesi ile iletişim sağlama gibi.. </li>
</ul>
NOT: AngularJS' e başlamadan önce HTML, CSS ve Javascript hakkında biraz bilgi sahibi olmanız gerekir.
<h2>AngularJS Kurulumu</h2>
Angular kütüphanesi kurulmadan önce NodeJs programı ve NPM kütüphanesi bilgisayarda yüklü olması gerekir.
<h4> NodeJS Kurulumu</h4>
NodeJS kurulumu için <a href="https://nodejs.org/en/">NodeJS</a> resmi web sayfasından bilgisayarımıza indirip kolay bir şekilde kurubiliriz.<br>
Kurulum işlemi bittikten sonra bir dosya oluşturup <b><i>windows işletim sistemlerinin komut satırı(cmd)</i></b> veya <b><i>Visual Stadio</i></b> programın terminal kısmına 
<b><i>npm init</i></b> yazarak önümüze gelen gelen soruları yanıtlayarak ya da <b><i>npm init --yes</i></b> diyerekten Package.json dosyası yüklenilir.<br>
<b><i>Package.json</i></b> : Uygulama bilgilerini ve paket bilgilerini yönetebileceğimiz paket dosyasıdır.<br>
<h3>AngularJS Kurulumu</h3>
<b><i>windows işletim sistemlerinin komut satırı(cmd)</i></b> veya <b><i>Visual Stadio</i></b> programın terminal kısmına 
<b><i>npm install -g @angular/cli</i></b> komut satırı çalıştırarak angular kütüphanesi yüklenilir veya <b><i>npm install -g @angular/cli@</b>verisiyon</i> şeklinde indirmek istediğimiz versiyonu belirtebiliriz. <br>
<h2>İlk Uygulama</h2>
<ul>
  <li><b><i>cd desktop</i></b> masaüstüne geçiş yapılır</li>
  <li><b><i>ng help</i></b> ng ile yapabileceğimiz işlemler gelir. Örneğin bir dosya oluşturmak gibi...</li>
  <li><b><i>ng new AngularJS</i></b> AngularJS adında bir dosya oluşturur.</li>
  <li><b><i>cd AngularJS</i></b> AngularJS klasörüne giriş yapılır</li>
  <li><b><i>code .</i></b> ile bizim kullanacağımız editör gelir(Visual Stadio) </li>
  <li><b><i>ng serve</i></b> proje çalıştırılır.</li>
</ul>
<h1>AngularJS Giriş</h1>
AngularJS, HTML'yi ng yönergeleriyle genişletir .<br>
<ul>
  <li><b><i>ng-app </i></b>bir AngularJS uygulamasını tanımlar . </li>
  <li><b><i>ng-model  </i></b> HTML kontrollerinin (input, select, textarea) değerini uygulama verilerine bağlar. [(ngModel)]='...' şeklinde kullanılır ve app.module.ts içerisinde export edilir.</li>
  <li><b><i>ng-bind </i></b>uygulama verilerini HTML görünümüne bağlar . </li>
  <li><b><i>ng-init </i></b>AngularJS uygulama değişkenlerini başlatır.  </li>
  <li><b><i>{{ ifade }}</i></b> AngularJS ifadeleri çift parantez içinde yazılır .</li>
</ul>

<a href="https://www.w3schools.com/angular/default.asp">w3schools</a> <br>

<h2>[(ngModel)] Şablona dayalı formlar</h2>
<br><a href="https://angular.io/guide/forms-overview">Formlar</a><br><br>
Kullanıcı girdisini formlarla işlemek, birçok yaygın uygulamanın temel taşıdır. 
Uygulamalar, kullanıcıların oturum açmasını, bir profili güncellemesini, hassas bilgileri girmesini ve diğer birçok veri girişi görevini gerçekleştirmesini sağlamak için formları kullanır.<br>
<b><i>Reaktif formlar</i></b> , temel alınan formlar nesne modeline doğrudan, açık erişim sağlar. Şablon temelli formlarla karşılaştırıldığında, daha sağlamdırlar: daha ölçeklenebilir, yeniden kullanılabilir ve test edilebilirler.<br>
<b><i>Şablona dayalı formlar</i></b> , temel alınan nesne modelini oluşturmak ve işlemek için şablondaki yönergelere dayanır. E-posta listesi kayıt formu gibi bir uygulamaya basit bir form eklemek için kullanışlıdırlar. Bir uygulamaya eklemek kolaydır, ancak reaktif formlar kadar iyi ölçeklenmezler.<br><br>
<table>
  <thead>
    <tr>
      <th>Farkları </th>
      <th>REAKTİF [formControl]</th>
      <th>ŞABLON ODAKLI  [(NgModel)] </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Form modelinin kurulumu </td>
      <td>Açık, bileşen sınıfında oluşturuldu </td>
      <td>Direktifler tarafından oluşturulan örtük </td>
    </tr>
    <tr>
      <td>Veri örneği </td>
      <td>Yapılandırılmış ve değişmez </td>
      <td>Yapılandırılmamış ve değişken </td>
    </tr>
    <tr>
      <td>Veri akışı </td>
      <td>Senkron </td>
      <td>	asenkron </td>
    </tr>
    <tr>
      <td>Form doğrulama </td>
      <td>	Fonksiyonlar </td>
      <td> direktifler</td>
    </tr>
  </tbody>
</table>
  



Şablona dayalı formlar , şablonda değişiklikler yapıldıkça bileşendeki veri modelini güncellemek için <b><i>iki yönlü veri bağlamayı kullanır</i></b> ve bunun tersi de geçerlidir.

