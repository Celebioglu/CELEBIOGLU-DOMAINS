# EstiBot API Entegrasyonu Rehberi

## 1. Genel Bakış
EstiBot API, domain bilgilerini (appraisal, whois, leads) programatik olarak JSON formatında almanı sağlar. Base URL: https://api.estibot.com

**Resmi Dokümantasyon**: https://github.com/domainret/estibot-api (2026 güncel)

## 2. Erişim ve Fiyatlandırma
- **Ücretsiz**: Sınırlı sorgu
- **Advanced Plan**: $99/ay → 5,000 lookup/gün, 150,000/ay
- API key ile authentication

## 3. Temel Kullanım

### Örnek Sorgu (Appraisal)
```bash
curl -X GET "https://api.estibot.com/v1/appraise?domain=example.com&api_key=YOUR_KEY"
```

**Dönen JSON Örneği**:
```json
{
  "domain": "example.com",
  "appraised_value": 2500,
  "comparable_sales": [...],
  "keywords": [...],
  "backlinks": 120
}
```

## 4. Senin Sistemine Entegrasyon
- **Python Script**: Haftalık portföy valuation raporu üret
- **Zapier/Make**: Yeni domain eklendiğinde otomatik appraisal
- **Dashboard**: Streamlit veya Google Sheets ile görselleştir
- **Repo Entegrasyonu**: valuation.md ile birleştir, toplu raporlar üret

## 5. Avantajlar (CELEBIOGLU-DOMAINS için)
- Binlerce domain'i hızlı değerlendir
- Lead generation (potansiyel alıcılar)
- Otomatik portföy takibi
- Alüminyum/Marine nişine özel filtreleme

**Not**: API kullanımı için EstiBot sitesinden kayıt ol ve key al. Etik kullanım: rate limit'lere dikkat et.

---

*Repo entegrasyonu: estibot_api_guide.md*