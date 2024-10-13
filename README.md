# MODOKO
2025 Patika.dev Web3 Stajı
//hesap makinesi
//değişken (let-->immutable, var-->mutable )
//operatörler
//async metodu
//if condition


//canester --> akıllı sözleşme

actor hesap_makinesi{
var hucre: Int=0;

//toplama
//fonksiyon
public func toplama(s: Int) : async Int {
  hucre += s;
  hucre
  //(Debug.print(debug_show (hucre));)
};
//çıkarma
public func cikarma(s: Int) : async Int{
  hucre -= s;
  hucre
};
//çarpma
public func carpma(s: Int)  : async Int{
  hucre *= s;
  hucre
};
//bölme
public func bolme(s: Int)  : async ?Int{
  if ( s == 0){
    null
  }else{
    hucre /= s;
    ?hucre
  };
};

//temizle
public func temizle(): async (){
  hucre := 0 ;
};

};
