![banner](https://github.com/emirkabal/deprem-api/blob/master/.github/banner.jpg?raw=true)

# deprem-api
### Parametreler:
- **type** : Depremlerin hangi kaynaktan alınacağını belirtir. "afad", "kandilli" (varsayılan: kandilli)
- **size** : Depremin büyüklüğüne göre filtreleme yapar.
- **location** : Depremin lokasyonuna göre filtereleme yapar.
- **hour** : Depremin kaç saat önce gerçekleştiğine göre filtereleme yapar.


### Örnekler:
- https://deprem-api.vercel.app
- https://deprem-api.vercel.app/?type=afad
- https://deprem-api.vercel.app/?size=3.1
- https://deprem-api.vercel.app/?location=istanbul
- https://deprem-api.vercel.app/?size=3.1&location=istanbul
- https://deprem-api.vercel.app/?hour=2
- https://deprem-api.vercel.app/?size=3.1&hour=2
- https://deprem-api.vercel.app/?size=3.1&hour=2&location=istanbul

## JSON Çıktısı:
```jsonc
"earthquakes": [
    {
      "id": 1,
      "date": "2022.09.05 16:45:54", // GMT+3
      "timestamp": 1662385554,
      "latitude": 37.1075,
      "longitude": 28.5117,
      "depth": 2.8, // km
      "size": {
        "md": 0.0,
        "ml": 3.6,
        "mw": 3.7
      },
      "location": "ARMUTCUK-ULA (MUGLA)",
      "attribute": "İlksel"
    }, {...}
]
```
## Bilgilendirme
**deprem-api** aşağıdaki referanslar kullanılarak oluşturulmuştur ve tüm verileri aşağıda belirtilen kaynaklardan almaktadır.
### Referanslar:
- [AFAD (Türkiye Afet ve Acil Durum Yönetimi Başkanlığı)](https://www.afad.gov.tr/)
- [Kandi̇lli̇ Rasathanesi̇ ve Deprem Araştırma Ensti̇tüsü](http://www.koeri.boun.edu.tr/sismo/2/en/)
