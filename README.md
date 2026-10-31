<!-- ========================= HEADER ========================= -->
**Полный код — замени им содержимое `README.md` профиля.** H&M вынесен отдельным блоком над стеком и остальными проектами.

```markdown
<p align="center">
  <img
    src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=2500&pause=800&color=38BDF8&center=true&vCenter=true&width=750&lines=Hi%2C+I'm+Vlad+%F0%9F%91%8B;Data+Science+%7C+Machine+Learning;ML+Engineering+%7C+MLOps"
    alt="Hi, I'm Vlad — Data Science and Machine Learning"
  />
</p>

<p align="center">
  <b>Data Science • Machine Learning • ML Engineering • MLOps</b>
</p>

<br>

<!-- CONTACTS -->

<p align="center">
  <a href="https://t.me/Edgrel">
    <img
      src="https://img.shields.io/badge/Telegram-@Edgrel-26A5E4?style=for-the-badge&logo=telegram&logoColor=white"
      alt="Telegram"
    />
  </a>
  <a href="mailto:misterxplot@gmail.com">
    <img
      src="https://img.shields.io/badge/Email-misterxplot%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white"
      alt="Email"
    />
  </a>
  <a href="https://github.com/misterxplot-cmd">
    <img
      src="https://img.shields.io/badge/GitHub-misterxplot--cmd-181717?style=for-the-badge&logo=github&logoColor=white"
      alt="GitHub"
    />
  </a>
</p>

<p align="center">
  <img
    src="https://komarev.com/ghpvc/?username=misterxplot-cmd&style=for-the-badge&color=0e75b6&label=PROFILE+VIEWS"
    alt="Profile Views"
  />
</p>

---

# 💼 Практический опыт в ML

## Прогнозирование повторных покупок клиентов H&M

**Самостоятельная ML-разработка · Октябрь 2026**

[![CI](https://github.com/misterxplot-cmd/hm-repeat-purchase-ml/actions/workflows/ci.yml/badge.svg)](https://github.com/misterxplot-cmd/hm-repeat-purchase-ml/actions)

Прогноз покупки клиента в следующие **30 дней** по истории
его поведения за предыдущие **90 дней**.

### Данные и реализация

- Загрузил в PostgreSQL **31,8 млн товарных записей**
  по **1,36 млн клиентов**.
- Построил SQL-витрину из **10,7 млн клиентских срезов**.
- Выполнил аудит данных, агрегацию до уровня «клиент-день»,
  проверки кардинальности JOIN и сохранения числа строк и сумм.
- Подготовил признаки частоты, давности и средней суммы покупок
  в исходной шкале `price`.
- Сравнил recency baseline, LogisticRegression и CatBoost
  на трёх временных срезах.
- Выполнил калибровку вероятностей, финальное тестирование
  и пакетный расчёт клиентских прогнозов.
- Добавил CLI, **43 теста**, включая интеграционные
  с PostgreSQL и сквозной прогон, и CI в GitHub Actions.

### Результаты

Финальный тест: **539 884 клиента**.
Выбранная модель: **CatBoost с тремя признаками**.

| Метрика | Recency baseline | CatBoost |
|---|---:|---:|
| Average Precision | 0,4053 | 0,5345 |
| ROC-AUC | 0,6143 | 0,6876 |
| Precision@5% | 49,00% | **75,09%** |
| Lift@5% | 1,564 | **2,396** |

Верхние 5% списка — **26 995 клиентов**.
Прирост Precision@5% относительно baseline — **26,09 п.п.**

### Стек

`Python` `SQL` `PostgreSQL` `pandas` `NumPy`
`scikit-learn` `CatBoost` `Docker` `pytest` `GitHub Actions`

<p>
  <a href="https://github.com/misterxplot-cmd/hm-repeat-purchase-ml">
    <img
      src="https://img.shields.io/badge/Код_и_запуск-181717?style=for-the-badge&logo=github&logoColor=white"
      alt="Код и запуск"
    />
  </a>
  <a href="https://github.com/misterxplot-cmd/hm-repeat-purchase-ml/blob/main/reports/results.md">
    <img
      src="https://img.shields.io/badge/Результаты-2563EB?style=for-the-badge"
      alt="Результаты экспериментов"
    />
  </a>
  <a href="https://github.com/misterxplot-cmd/hm-repeat-purchase-ml/releases">
    <img
      src="https://img.shields.io/badge/Модели-15803D?style=for-the-badge"
      alt="Обученные модели"
    />
  </a>
</p>

---

# 🧠 Tech Stack

### Languages & Databases

<p align="center">
  <a href="https://www.python.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/python/python-original.svg"
      width="52" height="52" alt="Python"
    />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.postgresql.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/postgresql/postgresql-original.svg"
      width="52" height="52" alt="PostgreSQL"
    />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
</p>

---

### Data Science & Machine Learning

<p align="center">
  <a href="https://pandas.pydata.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/pandas/pandas-original.svg"
      width="52" height="52" alt="pandas"
    />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://numpy.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/numpy/numpy-original.svg"
      width="52" height="52" alt="NumPy"
    />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://scikit-learn.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/scikitlearn/scikitlearn-original.svg"
      width="52" height="52" alt="scikit-learn"
    />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="pandas" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="scikit-learn" />
  <img src="https://img.shields.io/badge/CatBoost-FFCC00?style=for-the-badge&logoColor=black" alt="CatBoost" />
  <img src="https://img.shields.io/badge/CatBoostRanker-FFD700?style=for-the-badge&logoColor=black" alt="CatBoostRanker" />
  <img src="https://img.shields.io/badge/Optuna-4F46E5?style=for-the-badge&logoColor=white" alt="Optuna" />
</p>

---

### Big Data & Data Engineering

<p align="center">
  <a href="https://spark.apache.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/apachespark/apachespark-original.svg"
      width="58" height="58" alt="Apache Spark"
    />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://airflow.apache.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/apacheairflow/apacheairflow-original.svg"
      width="58" height="58" alt="Apache Airflow"
    />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="Apache Spark" />
  <img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="PySpark" />
  <img src="https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apacheairflow&logoColor=white" alt="Apache Airflow" />
</p>

---

### ML Engineering & MLOps

<p align="center">
  <a href="https://mlflow.org/">
    <img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white" alt="MLflow" />
  </a>
  <img src="https://img.shields.io/badge/Machine%20Learning-0F172A?style=for-the-badge&logoColor=white" alt="Machine Learning" />
  <img src="https://img.shields.io/badge/ML%20Engineering-312E81?style=for-the-badge&logoColor=white" alt="ML Engineering" />
  <img src="https://img.shields.io/badge/MLOps-0F766E?style=for-the-badge&logoColor=white" alt="MLOps" />
</p>

---

### Development & Infrastructure

<p align="center">
  <a href="https://www.docker.com/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original.svg"
      width="55" height="55" alt="Docker"
    />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://git-scm.com/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/git/git-original.svg"
      width="55" height="55" alt="Git"
    />
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;
  <a href="https://www.linux.org/">
    <img
      src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/linux/linux-original.svg"
      width="55" height="55" alt="Linux"
    />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux" />
</p>

---

# 🚀 Key Projects

<details>
<summary>
  <b>🛡 transaction-risk-api</b> — ML Inference API
</summary>

<br>

API-сервис для инференса учебной модели оценки риска транзакций.

### What I did

- strict input validation
- single and batch prediction
- model loading and readiness checks
- ML model inference
- API testing

### Stack

`Python` `FastAPI` `Pydantic` `scikit-learn` `pytest`

<br>

<a href="https://github.com/misterxplot-cmd/transaction-risk-api">
  <img
    src="https://img.shields.io/badge/Open%20Repository-181717?style=for-the-badge&logo=github&logoColor=white"
    alt="Open transaction-risk-api"
  />
</a>

</details>

<br>

<details>
<summary>
  <b>⚡ numba-session-features</b> — High Performance Feature Engineering
</summary>

<br>

Расчёт признаков пользовательских сессий на синтетических данных
и сравнение Python-циклов с Numba.

### What I did

- Numba JIT optimization
- separate compilation and warm-run measurements
- feature calculation correctness checks
- performance benchmarking
- ML classification pipeline

### Stack

`Python` `NumPy` `pandas` `Numba` `scikit-learn`

<br>

<a href="https://github.com/misterxplot-cmd/numba-session-features">
  <img
    src="https://img.shields.io/badge/Open%20Repository-181717?style=for-the-badge&logo=github&logoColor=white"
    alt="Open numba-session-features"
  />
</a>

</details>

<br>

<details>
<summary>
  <b>📊 transaction-risk-ml</b> — Transaction Risk Classification
</summary>

<br>

Учебная классификация риска транзакций:
сравнение наборов признаков и проверка утечек данных.

### What I did

- exploratory data analysis
- preprocessing pipelines
- feature engineering
- model training and validation
- comparison of feature sets
- data leakage analysis

### Stack

`Python` `pandas` `NumPy` `scikit-learn`

<br>

<a href="https://github.com/misterxplot-cmd/transaction-risk-ml">
  <img
    src="https://img.shields.io/badge/Open%20Repository-181717?style=for-the-badge&logo=github&logoColor=white"
    alt="Open transaction-risk-ml"
  />
</a>

</details>

<br>

<details>
<summary>
  <b>📈 dutch-auction</b> — Dutch Auction Simulation
</summary>

<br>

Учебный симулятор голландского аукциона на Python
с синтетической историей цен.

### What I did

- object-oriented model: Lot, Agent, Auction
- implemented 5 agent strategies
- fair value estimation
- synthetic price generation with mean reversion
- auction simulation and visualization

### Stack

`Python` `OOP` `Matplotlib`

<br>

<a href="https://github.com/misterxplot-cmd/dutch-auction">
  <img
    src="https://img.shields.io/badge/Open%20Repository-181717?style=for-the-badge&logo=github&logoColor=white"
    alt="Open dutch-auction"
  />
</a>

</details>

---

# 🎯 Focus Areas

<p align="center">
  <img src="https://img.shields.io/badge/Feature%20Engineering-581C87?style=for-the-badge" alt="Feature Engineering" />
  <img src="https://img.shields.io/badge/Temporal%20Validation-1D4ED8?style=for-the-badge" alt="Temporal Validation" />
  <img src="https://img.shields.io/badge/Customer%20Analytics-15803D?style=for-the-badge" alt="Customer Analytics" />
  <img src="https://img.shields.io/badge/Ranking-7E22CE?style=for-the-badge" alt="Ranking" />
  <img src="https://img.shields.io/badge/Risk%20Scoring-B91C1C?style=for-the-badge" alt="Risk Scoring" />
  <img src="https://img.shields.io/badge/Data%20Processing-0F766E?style=for-the-badge" alt="Data Processing" />
</p>

---

<p align="center">
  <a href="https://github.com/misterxplot-cmd?tab=repositories">
    <img
      src="https://img.shields.io/badge/VIEW%20ALL%20PROJECTS-181717?style=for-the-badge&logo=github&logoColor=white"
      alt="View all repositories"
    />
  </a>
</p>
```

