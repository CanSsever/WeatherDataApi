# 🌤️ Weather API

This is a simple RESTful Weather API built with Flask and Pandas.  
It allows you to access temperature data for various weather stations by date, station ID, or year.

## 📦 Features

- List all available weather stations
- Get the temperature for a specific station and date
- Fetch all temperature data for a station
- Get yearly temperature records for a station

## 🛠️ Technologies Used

- Python 🐍
- Flask 🚀
- Pandas 📊

## 📁 File Structure

.
├── datasmall/
│ ├── stations.txt
│ └── TG_STAIDxxxxxx.txt
├── templates/
│ └── home.html
├── app.py
└── README.md



## ▶️ How to Run

1. Clone the repository:
git clone https://github.com/yourusername/weather-api.git
cd weather-api



2. Install dependencies:
pip install flask pandas



3. Run the app:
python app.py



4. Visit in browser:
http://localhost:5000/



## 📌 API Endpoints

### `GET /`
- Displays all available stations as an HTML table.

### `GET /api/v1/<station>/<date>`
- Returns temperature data for the given station and date.
- Example: `/api/v1/10/1990-01-01`

### `GET /api/v1/<station>`
- Returns all temperature data for the given station.
- Example: `/api/v1/10`

### `GET /api/v1/yearly/<station>/<year>`
- Returns temperature records for the station in a specific year.
- Example: `/api/v1/yearly/10/1990`

## 📌 Notes

- Temperature values are stored in tenths of °C and converted to °C.
- Invalid station IDs or dates return empty JSON or error.

## 📄 License

MIT License

## 🙋‍♂️ Author

Created by ** Can Sever**  
Feel free to reach out or contribute!