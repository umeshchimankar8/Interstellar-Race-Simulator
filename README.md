# Interstellar-Race-Simulator

Two space agencies, NASA and ESA, are in a race to explore a series of
exoplanets. Each agency launches probes to these planets. The competition
works as follows:
1. For each planet, both agencies launch a probe simultaneously.
2. An agency gains a 'discovery point' if their probe reaches the planet faster
than their opponent's.
3. If both probes reach the planet at the same time, neither agency gains a
point.
4. The first agency to gain 7 discovery points wins the race.
5. If neither agency reaches 7 points after visiting all planets, the result is a
'No Winner'.
6. Each probe has two stats: speed (km/h) and fuel efficiency (light-years/unit).
The agency whose probe has a higher value when speed is multiplied by fuel
efficiency reaches the planet first. Within a sub-array, the first 2 values are for
probe NASA and next 2 values are for ESA.
Write a Python function that simulates this space race and returns the winner
('NASA', 'ESA', or 'No_Winner').

# Sample Input:
planets = 4
results = [[100000, 2.5, 90000, 3.0], [120000, 2.0, 100000, 2.2], [80000, 3.5,
95000, 3.0], [110000, 2.8, 105000, 3.1]]

# Sample Output:
No_Winner

# Explanation:
After 4 planet visits:
- NASA wins for planet 2 (120000 * 2.0 > 100000 2.2)
- ESA wins for planets 1, 3, and 4
ESA has 3 points, NASA has I point, but neither reaches 7, so ESA leads
but the race continues.
