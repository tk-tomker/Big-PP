# 🏉 Fantasy School Sports – Project Roadmap

## 🧭 Project Overview

Each player picks **5 school teams** (e.g. 1st XV, U15A, U18B).  
Each real-world team earns or loses points based on **match results** (points difference).  
Each player’s total score = the **sum of the points differences** for their chosen teams.

---

## 🚀 Phase 1: Planning and Setup

### Objectives
- Define how the game will work.
- Design the basic structure of the program.
- Assign teams and roles.

### Tasks
1. **Define Core Rules**
   - How many school teams exist?
   - How are match results entered? (manually by admin?)
   - How often are scores updated? (weekly?)

2. **Design Data Structures**
   - Represent school teams and their match results.
   - Represent users/players and their chosen teams.
   - Store total points per user.

3. **Decide Storage Method**
   - Simple: text file (`teams.txt`, `players.txt`)
   - Medium: CSV or JSON file
   - Advanced: SQLite database

4. **Assign Roles (Example)**
   - **Team A**: User Interface (menu, inputs, outputs)
   - **Team B**: Game Logic (calculating scores)
   - **Team C**: Data Storage (saving/loading)
   - **Team D**: Admin System & Validation
   - **Team E**: Testing & Documentation

---

## 🧩 Phase 2: Core System Development

### 1. Data Models (Team C)
Create Python classes or dictionaries:

```python
class Team:
    def __init__(self, name):
        self.name = name
        self.total_points = 0
```

```python
class Player:
    def __init__(self, name, chosen_teams):
        self.name = name
        self.chosen_teams = chosen_teams
        self.score = 0
```

- Store data in lists or files.
- Add functions to save and load data (JSON or CSV).

---

### 2. Game Logic (Team B)
- Function to input match results:
```python
def update_team_score(team_name, points_difference):
    # Adds/subtracts points from that team’s total
```

- Function to calculate each player’s total score based on their teams.
- Handle weekly updates.

---

### 3. User Interface (Team A)
Create simple console menus:

```
1. Create Player
2. Pick Teams
3. View Leaderboard
4. Update Match Results (admin)
```

Display player stats and leaderboards clearly.

---

### 4. Admin System (Team D)
- Allow admin login.
- Admin can input match results for each school team.
- Results automatically update all player scores.

---

## 🧪 Phase 3: Integration and Testing

### Objectives
- Combine all team modules.
- Debug data flow.
- Ensure scoring updates work correctly.

### Tasks
- Merge all modules together.
- Create a sample dataset (e.g. 6 teams, 3 players).
- Simulate one “week” of results.
- Test for:
  - Player creation
  - Team selection
  - Result updating
  - Leaderboard updating

---

## 🎨 Phase 4: Polish and Extras (Optional)

Add optional features if time allows:
- 🏆 Weekly leaderboard / rankings  
- 📊 Graphs of score changes (using `matplotlib`)  
- 💾 Persistent storage (SQLite database)  
- 🌐 Simple web version (using Flask or Streamlit)  
- 🎯 Error handling (invalid inputs, duplicate teams)

---

## 📘 Phase 5: Documentation & Presentation

Each subteam prepares:
- A short explanation of their code and design choices.
- Comments inside code and a `README.md`.
- Example runs or screenshots.
- Group demo showing how all parts work together.

---

## 🧠 Suggested Timeline (4–6 Weeks)

| Week | Focus | Outcome |
|------|--------|----------|
| 1 | Planning + Design | Rules defined, roles assigned, structure agreed |
| 2 | Data Models + File Handling | Teams and players stored and loaded |
| 3 | Implement Scoring Logic | Scores correctly update with match results |
| 4 | User Interface + Admin System | Full game playable in console |
| 5 | Integration + Testing | Bug fixes, consistent data flow |
| 6 | Documentation + Demo | Polished code and group presentation |

---

## ✅ Deliverables Checklist

- [ ] Team & player data structures working  
- [ ] Match results update correctly  
- [ ] Player scores recalculate automatically  
- [ ] Menu-based UI functional  
- [ ] Data persists between runs  
- [ ] Basic error handling  
- [ ] Documented, commented code  
- [ ] Presentation/demo ready  

---

## 🔜 Optional Next Step

Create a **visual project flowchart** showing how data moves:
- Admin → Results → Teams → Players → Leaderboard

(Recommended for helping students understand how the modules connect.)

---
