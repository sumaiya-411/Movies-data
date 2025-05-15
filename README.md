# Movie Data Analysis with DuckDB

This project demonstrates how to use [DuckDB](https://duckdb.org/) in a Jupyter notebook to analyze movie data stored in a local CSV file. The focus is on filtering and sorting data — for example, extracting all comedy movies and ordering them by release date.

## Project Structure

```
├── movies.csv               # Sample movie dataset
├── analysis.ipynb           # Jupyter notebook with DuckDB queries
└── README.md                # Project documentation
```

## Requirements

- Python 3.7+
- DuckDB
- JupyterLab or Jupyter Notebook

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/duckdb-movie-analysis.git
   cd duckdb-movie-analysis
   ```

2. Install dependencies (if not already installed):

   ```bash
   pip install duckdb jupyterlab
   ```

3. Launch JupyterLab:

   ```bash
   jupyter lab
   ```

## Usage

1. Open `analysis.ipynb`.
2. Make sure `movies.csv` is in the same directory.
3. Run the cells to query the data using DuckDB.

## Example Query
mmn.
```sql
SELECT *
FROM read_csv_auto('movies.csv')
WHERE Genre = 'Comedy'
ORDER BY "Release Date" DESC;
```

## License

This project is licensed under the MIT License.
