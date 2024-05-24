def count_valid_teams(n, team_sizes):
    valid_teams = 0
    for size in team_sizes:
        if size % 3 == 0 and size > 0:
            valid_teams += 1
    return valid_teams

n = int(input())
team_sizes = [int(input()) for _ in range(n)]

print(count_valid_teams(n, team_sizes))

