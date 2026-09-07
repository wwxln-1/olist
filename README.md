# Olist E-Commerce Data Analytics — BTEC HND Assignment

**Pearson BTEC Higher Nationals in Digital Technologies**
Unit 12: Data Analytics | Unit Code: K/615/1637 | Level 4 / 15 Credits

Ushbu repository Olist (Brazilian E-Commerce) datasetiga asoslangan uch bosqichli data analytics topshirig'ini o'z ichiga oladi: nazariy asos, deskriptiv tahlil va predictive (bashoratli) tahlil. Ish Jupyter Notebook (`olist_assigment.ipynb`) ko'rinishida taqdim etilgan va assessment criteria (P1–P6, M1–M3, D1–D2) bo'yicha tuzilgan.

## 📌 Loyiha tuzilishi (Tasklar)

### 🔷 Task 1 — Theoretical Foundation of Data Analytics (`P1`, `P2`, `M1`, `D1`)
- Data analytics ta'rifi va biznesdagi roli
- Asosiy statistik atamalar (population, sample va h.k.) dataset misollari bilan
- Python va Jupyter Notebook vositalarini tanishtirish
- Olist datasetini yuklash va yagona `main` DataFrame'ga birlashtirish (merge)
- Ustunlar tavsifi va ma'lumot turlari jadvali
- Uch turdagi analitika (descriptive, predictive, prescriptive) va sanoat misollari
- Qaror qabul qilishda data analytics ahamiyatini tanqidiy baholash

### 🔷 Task 2 — Descriptive Analytics: Understanding Current Performance (`P3`, `P4`, `M2`)
- O'zgaruvchilarni turkumlash (nominal, discrete, continuous, datetime)
- Yetishmayotgan qiymatlarni tahlil qilish
- Univariate tahlil: Revenue taqsimoti (histogram), mahsulot kategoriyalari chastotasi (bar chart)
- Bivariate tahlil: Price vs Freight Value (scatter plot)
- Markaziy tendensiya (mean, median, mode) va dispersiya (range, variance, std) o'lchovlari
- Kvartillar, IQR orqali outlierlarni aniqlash, boxplot vizualizatsiyasi
- 10% tasodifiy sample va to'liq populyatsiya taqqoslanishi
- Oylik daromad trendi (time series) tahlili
- Deskriptiv natijalarni aniq biznes qarorlari bilan bog'lash

### 🔷 Task 3 — Predictive Analytics: Forecasting Future Events (`P5`, `P6`, `M3`, `D2`)
- Simple Linear Regression: Price → Revenue
- Multiple Linear Regression: Price + Freight → Revenue (R², MAE, RMSE baholash)
- Korrelyatsiya matritsasi va heatmap
- Forecasting usul 1: 3 oylik Moving Average (harakatlanuvchi o'rtacha)
- Forecasting usul 2: Simple Exponential Smoothing (SES)
- Predictive usullarni solishtirish jadvali
- Model natijalarini (masalan, R² = 0.9943) tanqidiy baholash — ma'lumot sifati, model taxminlari va mas'uliyatli qo'llash nuqtai nazaridan

## 🛠 Ishlatilgan texnologiyalar

- Python 3
- pandas, numpy
- matplotlib, seaborn
- scipy (`stats`, `optimize`)
- scikit-learn (`LinearRegression`, `r2_score`, `mean_absolute_error`, `mean_squared_error`)
- Jupyter Notebook

## 📂 Loyiha tuzilishi

```
.
├── olist_assigment.ipynb                    # Asosiy topshiriq notebook fayli
├── olist_orders_dataset.csv                 # Buyurtmalar
├── olist_order_items_dataset.csv            # Buyurtma tarkibidagi mahsulotlar
├── olist_products_dataset.csv               # Mahsulotlar
├── olist_customers_dataset.csv              # Mijozlar
├── olist_order_payments_dataset.csv         # To'lovlar
├── olist_sellers_dataset.csv                # Sotuvchilar
├── olist_order_reviews_dataset.csv          # Sharhlar/baholar
└── README.md                                # Ushbu fayl
```

> ⚠️ **Eslatma:** Olist datasetining barcha 7 ta CSV fayli notebook bilan bir papkada bo'lishi shart, chunki `pd.read_csv()` orqali nomlari bo'yicha to'g'ridan-to'g'ri yuklanadi. Rasmiy dataset [Kaggle — Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) sahifasidan yuklab olinishi mumkin.

## 🚀 Loyihani ishga tushirish

1. Repository'ni klonlang:
   ```bash
   git clone https://github.com/<username>/<repo-nomi>.git
   cd <repo-nomi>
   ```

2. Kerakli kutubxonalarni o'rnating:
   ```bash
   pip install pandas numpy matplotlib seaborn scipy scikit-learn jupyter
   ```

3. Olist CSV fayllarini shu papkaga joylashtiring (agar hali yo'q bo'lsa, Kaggle'dan yuklab oling).

4. Jupyter Notebook'ni ishga tushiring:
   ```bash
   jupyter notebook
   ```

5. `olist_assigment.ipynb` faylini oching va katakchalarni ketma-ket bajaring.

## 📊 Asosiy natijalar (qisqacha)

- Revenue taqsimoti kuchli o'ng tomonga siljigan (right-skewed): o'rtacha R$140.64, mediana R$92.32
- IQR usuli orqali sezilarli miqdorda statistik outlierlar aniqlangan
- Price va Revenue o'rtasida juda yuqori chiziqli bog'liqlik (Simple Linear Regression R² ≈ 0.9943)
- Multiple Linear Regression (Price + Freight) modeli aniqlikni yanada oshirdi
- 3 oylik Moving Average va Exponential Smoothing usullari oylik daromad trendini bashorat qilish uchun solishtirildi

## 📚 Foydalanilgan adabiyotlar

Notebook oxirida to'liq ro'yxat keltirilgan (Bruce & Bruce, Dietel, Few, James et al., Kirk, Knaflic, McKinney, Provost & Fawcett, Wilke va boshqalar).

## 📄 Litsenziya

Ushbu loyiha ta'lim (BTEC HND assessment) maqsadida yaratilgan.
