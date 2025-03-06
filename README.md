# 👨‍💼 Исследование удовлетворенности сотрудников

## 📌 Описание проекта

Компания столкнулась с проблемой **снижения удовлетворенности сотрудников** и высокой **текучести кадров**.  
Было решено использовать **модель машинного обучения** для предсказания уровня удовлетворенности сотрудников и выявления факторов, влияющих на увольнения.  

🎯 **Цель исследования**:
1. **Разработать модель прогнозирования уровня удовлетворенности сотрудников**.
2. **Предсказать вероятность увольнения**.
3. **Выявить ключевые факторы, влияющие на удовлетворенность и текучесть кадров**.
4. **Предложить рекомендации по удержанию сотрудников**.

---

## 🎯 Основные задачи:
1. **Предобработка данных** (устранение пропусков, дубликатов, оптимизация типов данных).
2. **Анализ данных** (EDA, выявление зависимостей и ключевых факторов).
3. **Обучение моделей**:
   - **GradientBoostingRegressor** (для предсказания удовлетворенности).
   - **CatBoostClassifier** (для прогнозирования увольнений).
4. **Оценка качества моделей** (SMAPE, ROC-AUC, SHAP-анализ).
5. **Выявление профиля сотрудников с высоким риском увольнения**.
6. **Разработка рекомендаций для HR-отдела**.

---

## 📂 Содержание

[📌 Посмотреть проект можно здесь](project/hr_analaisis.ipynb)

---

## 🔬 Используемые методы и библиотеки

### 📚 **Библиотеки**:
- **pandas**, **numpy** – обработка данных
- **matplotlib**, **seaborn** – визуализация данных
- **scikit-learn**, **xgboost**, **lightgbm**, **catboost** – машинное обучение
- **shap** – интерпретация моделей
- **phik** – анализ корреляций

### 📊 **Методы анализа**:
- **Обработка данных**: устранение пропусков, выбросов, кодирование признаков.
- **Корреляционный анализ**: оценка мультиколлинеарности.
- **Обучение моделей**:
  - **GradientBoostingRegressor** (прогноз уровня удовлетворенности)
  - **CatBoostClassifier** (прогноз увольнения сотрудников)
- **Метрики оценки**:
  - **SMAPE** (Symmetric Mean Absolute Percentage Error)
  - **ROC-AUC** (качество классификации)
- **SHAP-анализ**: выявление значимости признаков.

---

## 📈 **Основные результаты**

🏆 **Выбранные модели**:
- **GradientBoostingRegressor** (предсказание уровня удовлетворенности).
- **CatBoostClassifier** (прогноз увольнений).

✅ **SMAPE на тестовой выборке (удовлетворенность):** **18.75%** (хорошая точность).  
✅ **ROC-AUC на тестовой выборке (увольнение):** **0.9240** (высокая точность).  
✅ **SHAP-анализ подтвердил значимость ключевых факторов**.  
✅ **Разработаны рекомендации для HR-отдела**.  

### 🔹 **Факторы, влияющие на удовлетворенность сотрудников**:
1️⃣ **Оценка руководителя (supervisor_evaluation)** – самый важный фактор.  
2️⃣ **Уровень должности (level)** – сотрудники с низкими позициями менее удовлетворены.  
3️⃣ **Стаж работы (employment_years)** – у новых сотрудников ниже уровень удовлетворенности.  

### 🔹 **Профиль сотрудника с высоким риском увольнения**:
- Молодой возраст.
- Низкая зарплата.
- Отсутствие повышения за прошлый год.
- Низкая загруженность.
- Низкий уровень удовлетворенности.

---

## 🔧 **Установка**

Для работы с проектом потребуется **Python 3.x** и следующие библиотеки:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm catboost shap phik
