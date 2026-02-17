# Entertainment Ratings

A personalized entertainment rating system for tracking movie, TV show, and music preferences for Sky and Tay. This dataset is optimized for use with ChatGPT to generate personalized recommendations based on individual ratings and favorites.

## 📁 Files

- **`entertainment_ratings.csv`** - CSV format, easily readable by ChatGPT and other AI tools
- **`entertainment_ratings.xlsx`** - Excel format with visual formatting for better readability
- **`create_xlsx.py`** - Python script to regenerate the XLSX file from CSV

## 📊 Data Structure

The spreadsheet contains the following columns:

| Column | Description |
|--------|-------------|
| **Type** | Category: Movie, TV Show, or Music Artist |
| **Title** | Name of the movie, TV show, or music artist |
| **Genre** | Genre classification (Drama, Sci-Fi, Comedy, Rock, Pop, etc.) |
| **Sky_Rating** | Sky's rating on a scale of 0-10 |
| **Tay_Rating** | Tay's rating on a scale of 0-10 |
| **Sky_Favorite** | TRUE if this is one of Sky's favorites (carries extra weight) |
| **Tay_Favorite** | TRUE if this is one of Tay's favorites (carries extra weight) |
| **Notes** | Additional context or comments about the entry |

## 🎯 How to Use with ChatGPT

### Getting Recommendations

1. **Upload the file**: Upload either `entertainment_ratings.csv` or `entertainment_ratings.xlsx` to ChatGPT
2. **Ask for recommendations**: Use prompts like:
   - "Based on Sky's ratings and favorites, recommend 5 movies they might enjoy"
   - "What TV shows would Tay like based on their preferences?"
   - "Suggest music artists similar to Landen's favorites"
   - "Find movies that all four people would enjoy watching together (rated 8+ by everyone)"
   - "What movies from the 2010s would Hanna enjoy based on their rating patterns?"

### Understanding the Weighting System

- **Favorites (TRUE flag)**: These entries carry extra weight in recommendations
- **High ratings (9.0+)**: Strong indicators of preference
- **Genre patterns**: ChatGPT can identify genre preferences and suggest accordingly
- **Both persons**: Find common ground by analyzing overlapping preferences

## ✏️ Adding New Entries

### Using CSV

Add new rows to `entertainment_ratings.csv` following this format:

```csv
Type,Title,Genre,Sky_Rating,Tay_Rating,Sky_Favorite,Tay_Favorite,Landen_Rating,Landen_Favorite,Hanna_Rating,Hanna_Favorite,Release_Year,Notes
Movie,Your Movie,Action,8.5,9.0,FALSE,TRUE,8.0,FALSE,9.5,TRUE,2023,Your notes here
```

### Using Excel

Open `entertainment_ratings.xlsx` and add rows directly. The file includes:
- Color-coded favorites (yellow highlight)
- High ratings highlighted (green for 9.0+)
- Formatted headers and borders
- Frozen header row for easy scrolling

### Regenerating XLSX from CSV

After editing the CSV, regenerate the formatted XLSX:

```bash
python3 create_xlsx.py
```

## 📝 Example Queries for ChatGPT

Here are some example prompts to get the most out of this data:

1. **Individual Recommendations**:
   - "What are Sky's top 5 favorite things based on this data?"
   - "Recommend TV shows for Tay similar to their favorites"

2. **Shared Recommendations**:
   - "What movies would both Sky and Tay enjoy? (Consider favorites)"
   - "Find common genres that both people rated highly"

3. **Discovery**:
   - "Suggest new music artists based on Sky's current favorites"
   - "What genres should Tay explore based on their rating patterns?"

4. **Analysis**:
   - "What are the rating differences between Sky and Tay?"
   - "Which person prefers sci-fi more?"
   - "Identify items where ratings differ by more than 1 point"

## 🔧 Customization

### Adding More People

To track ratings for additional people, add new columns:
- `PersonName_Rating`
- `PersonName_Favorite`

### Adding More Fields

Consider adding:
- Director/Creator/Band Members
- Streaming Platform
- Last Watched Date
- Rewatch Value
- Duration/Runtime

## 📦 Requirements

To regenerate the XLSX file, you need Python 3.x and openpyxl:

```bash
pip install openpyxl
```

## 🎬 Sample Data

The repository includes 30 sample entries:
- 10 Movies (including classics like The Shawshank Redemption, Inception, The Matrix)
- 10 TV Shows (Breaking Bad, Game of Thrones, Stranger Things, etc.)
- 10 Music Artists (The Beatles, Queen, Billie Eilish, etc.)

These samples demonstrate the rating system and can be replaced with your actual preferences.

## 📄 License

This is a personal project for entertainment tracking and recommendations.