# League2025WorldData
This project is to extract match stats for League of Legends 2025 World Main Play-In games and run analysis to understand the champion selections under the new Fearless Game mode

Most data were downloaded from OraclesElixir(https://oracleselixir.com/stats/champions/byTournament/2025%20Season%20World%20Championship%2FPlay-In)

Match data scraped from lol fandom(https://lol.fandom.com/Special:RunQuery/MatchHistoryGame?MHG%5Bpreload%5D=Tournament&MHG%5Bspl%5D=yes&MHG%5Btournament%5D=2025%20Season%20World%20Championship/Main%20Event&_run=) using code "match_scraper"


Clustering Analysis
============================================================
Champion Archetype Clustering by in-game stats(All Positions)
============================================================

=== CLUSTER 0 (2 champions) ===
=== Hypercarry ADC (outliers) ===
Champions: Jinx(ADC), Zeri(ADC)

Key characteristics:
  K/D/A: 8.0/1.0/9.5
  Kill Participation: 85.0%
  Damage%: 28.9%
  Gold%: 26.1%
  CS per Minute: 8.8
  First 10min Gold/XP/CS diff: -54 / -920 / -18

=== CLUSTER 1 (46 champions) ===
=== Carries with weak Lane phase ===
Champions: Aatrox(Top), Akali(Middle), Ambessa(Top), Anivia(Middle), Annie(Middle), Aurora(Middle), Aurora(Top), Azir(Middle), Camille(Top), Corki(ADC), Galio(Middle), Galio(Top), Gragas(Top), Ivern(Jungle), Jarvan IV(Jungle), 
Jax(Top), Jayce(Top), Jhin(ADC), K'Sante(Top), Kassadin(Middle), Kled(Top), Maokai(Jungle), Mordekaiser(Top), Naafiri(Jungle), Nocturne(Jungle), Ornn(Top), Pantheon(Jungle), Poppy(Jungle), Poppy(Top), Rek'Sai(Top), Rumble(Top), 
Sejuani(Jungle), Senna(ADC), Sion(Top), Sivir(ADC), Skarner(Jungle), Swain(Middle), Sylas(Middle), Syndra(Middle), Taliyah(Middle), Trundle(Jungle), Vi(Jungle), Viego(Jungle), Wukong(Jungle), Xin Zhao(Jungle), Yorick(Top)

Key characteristics:
  K/D/A: 2.8/3.1/5.9
  Kill Participation: 65.8%
  Damage%: 21.3%
  Gold%: 21.4%
  CS per Minute: 7.5
  First 10min Gold/XP/CS diff: -74 / -94 / -2

=== CLUSTER 2 (21 champions) ===
=== Support Champions ===
Champions: Alistar(Support), Bard(Support), Blitzcrank(Support), Braum(Support), Elise(Support), Karma(Support), Leona(Support), Lulu(Support), Morgana(Support), Nami(Support), Nautilus(Support), Neeko(Support), 
Pantheon(Support), Poppy(Support), Rakan(Support), Rell(Support), Renata Glasc(Support), Seraphine(Support), Soraka(Support), Tahm Kench(Support), Thresh(Support)

Key characteristics:
  K/D/A: 0.5/3.6/9.2
  Kill Participation: 75.5%
  Damage%: 8.7%
  Gold%: 9.7%
  CS per Minute: 1.0
  First 10min Gold/XP/CS diff: -7 / -57 / -0

=== CLUSTER 3 (33 champions) ===
=== Carries with winning lane ===
Champions: Ahri(Middle), Ashe(ADC), Caitlyn(ADC), Cassiopeia(Middle), Dr. Mundo(Jungle), Draven(ADC), Ezreal(ADC), Gnar(Top), Gwen(Top), Hwei(Middle), Kai'Sa(ADC), Kalista(ADC), LeBlanc(Middle), Lucian(ADC), Mel(Middle), Miss Fortune(ADC), 
Nidalee(Jungle), Orianna(Middle), Qiyana(Jungle), Renekton(Top), Ryze(Middle), Smolder(ADC), Smolder(Middle), Varus(ADC), Vayne(ADC), Viktor(Middle), Xayah(ADC), Yone(Middle), Yunara(ADC), Zed(Jungle), Ziggs(ADC), Ziggs(Middle), Zoe(Middle)

Key characteristics:
  K/D/A: 4.7/2.6/6.7
  Kill Participation: 70.2%
  Damage%: 26.9%
  Gold%: 24.6%
  CS per Minute: 8.7
  First 10min Gold/XP/CS diff: 202 / 196 / 5


============================================================
Meta Tier Classification
============================================================

Meta Tier Distribution:
Meta_Tier
A    14
B    33
C    48
S     7

S-Tier Champions (7):
Azir(Middle), Neeko(Support), Orianna(Middle), Poppy(Support), Poppy(Top), Sion(Top), Yunara(ADC)

A-Tier Champions (14):
Alistar(Support), Ambessa(Top), Bard(Support), Braum(Support), Corki(ADC), Ezreal(ADC), Jarvan IV(Jungle), Poppy(Jungle), Qiyana(Jungle), Rumble(Top), Taliyah(Middle), Trundle(Jungle), Wukong(Jungle), Xin Zhao(Jungle)

B-Tier Champions (33):
Akali(Middle), Aurora(Middle), Aurora(Top), Caitlyn(ADC), Cassiopeia(Middle), Draven(ADC), Galio(Middle), Galio(Top), Jax(Top), Jhin(ADC), K'Sante(Top), Kai'Sa(ADC), Karma(Support), LeBlanc(Middle), Leona(Support), Lucian(ADC), 
Nautilus(Support), Ornn(Top), Pantheon(Jungle), Rakan(Support), Rek'Sai(Top), Rell(Support), Renata Glasc(Support), Renekton(Top), Ryze(Middle), Sivir(ADC), Varus(ADC), Vi(Jungle), Viktor(Middle), Xayah(ADC), Yone(Middle), Ziggs(ADC), Ziggs(Middle)

C-Tier Champions (48):
Aatrox(Top), Ahri(Middle), Anivia(Middle), Annie(Middle), Ashe(ADC), Blitzcrank(Support), Camille(Top), Dr. Mundo(Jungle), Elise(Support), Gnar(Top), Gragas(Top), Gwen(Top), Hwei(Middle), Ivern(Jungle), Jayce(Top), Jinx(ADC), Kalista(ADC), 
Kassadin(Middle), Kled(Top), Lulu(Support), Maokai(Jungle), Mel(Middle), Miss Fortune(ADC), Mordekaiser(Top), Morgana(Support), Naafiri(Jungle), Nami(Support), Nidalee(Jungle), Nocturne(Jungle), Pantheon(Support), Sejuani(Jungle), Senna(ADC), 
Seraphine(Support), Skarner(Jungle), Smolder(ADC), Smolder(Middle), Soraka(Support), Swain(Middle), Sylas(Middle), Syndra(Middle), Tahm Kench(Support), Thresh(Support), Vayne(ADC), Viego(Jungle), Yorick(Top), Zed(Jungle), Zeri(ADC), Zoe(Middle)

Champion Synergy Study
================================================================================
INDIVIDUAL CHAMPION PERFORMANCE
================================================================================

🏆 TOP 10 MOST CONTESTED CHAMPIONS (Picks + Bans)
--------------------------------------------------------------------------------
Champion Position  Picks  Win_Rate  Pick_Rate  Ban_Rate  Presence
  Yunara      ADC     15      0.67      0.188     0.700        71
    Azir   Middle     14      0.50      0.175     0.637        65
 Orianna   Middle     19      0.58      0.238     0.563        64
   Neeko  Support     19      0.63      0.238     0.450        55
    Sion      Top     21      0.67      0.263     0.388        52
   Poppy  Support      8      0.88      0.100     0.538        51
 Alistar  Support     24      0.54      0.300     0.313        49
  Wukong   Jungle     21      0.57      0.263     0.350        49
   Poppy      Top      3      0.67      0.038     0.538        46
   Poppy   Jungle      2      0.50      0.025     0.538        45

⭐ TOP 10 HIGHEST WIN RATE CHAMPIONS (Min 5 picks)
--------------------------------------------------------------------------------
 Champion Position  Picks  Win_Rate
Dr. Mundo   Jungle      5      1.00
    Poppy  Support      8      0.88
     Yone   Middle      5      0.80
    Varus      ADC     13      0.77
   Yunara      ADC     15      0.67
     Sion      Top     21      0.67
    Galio   Middle      9      0.67
     Ornn      Top     11      0.64
    Neeko  Support     19      0.63
 Xin Zhao   Jungle     28      0.61

🚫 TOP 10 MOST BANNED CHAMPIONS
--------------------------------------------------------------------------------
Champion Position  Ban_Rate  Pick_Rate  Win_Rate
  Yunara      ADC     0.700      0.188      0.67
    Azir   Middle     0.637      0.175      0.50
 Orianna   Middle     0.563      0.238      0.58
   Poppy  Support     0.538      0.100      0.88
   Poppy      Top     0.538      0.038      0.67
   Poppy   Jungle     0.538      0.025      0.50
   Neeko  Support     0.450      0.238      0.63
    Sion      Top     0.388      0.263      0.67
  Wukong   Jungle     0.350      0.263      0.57
  Qiyana   Jungle     0.350      0.188      0.47


  
================================================================================
CHAMPION SYNERGY MATRIX
================================================================================

🔗 TOP ADC-SUPPORT SYNERGIES (Min 2 games)
--------------------------------------------------------------------------------
Corki           + Poppy           | 3 games | 100.0% WR
Ezreal          + Neeko           | 2 games | 100.0% WR
Corki           + Alistar         | 3 games | 100.0% WR
Varus           + Braum           | 2 games | 100.0% WR
Varus           + Poppy           | 2 games | 100.0% WR
Varus           + Rakan           | 2 games | 100.0% WR
Kalista         + Renata Glasc    | 2 games | 100.0% WR
Yunara          + Bard            | 2 games | 100.0% WR
Yunara          + Alistar         | 3 games | 100.0% WR
Corki           + Leona           | 4 games | 75.0% WR
Yunara          + Neeko           | 3 games | 66.7% WR
Kai'Sa          + Neeko           | 5 games | 60.0% WR
Caitlyn         + Neeko           | 5 games | 60.0% WR
Caitlyn         + Alistar         | 2 games | 50.0% WR
Sivir           + Leona           | 2 games | 50.0% WR

🔗 TOP JUNGLE-MID SYNERGIES (Min 2 games)
--------------------------------------------------------------------------------
Jarvan IV       + Yone            | 3 games | 100.0% WR
Xin Zhao        + LeBlanc         | 2 games | 100.0% WR
Xin Zhao        + Taliyah         | 4 games | 100.0% WR
Wukong          + Galio           | 3 games | 66.7% WR
Wukong          + Aurora          | 3 games | 66.7% WR
Trundle         + Orianna         | 3 games | 66.7% WR
Wukong          + Taliyah         | 5 games | 60.0% WR
Jarvan IV       + Orianna         | 5 games | 60.0% WR
Xin Zhao        + Orianna         | 7 games | 57.1% WR
Xin Zhao        + Azir            | 4 games | 50.0% WR
Pantheon        + Cassiopeia      | 2 games | 50.0% WR
Pantheon        + Taliyah         | 2 games | 50.0% WR
Jarvan IV       + Galio           | 4 games | 50.0% WR
Xin Zhao        + Anivia          | 2 games | 50.0% WR
Naafiri         + Orianna         | 2 games | 50.0% WR


================================================================================
COUNTER MATCHUP ANALYSIS
================================================================================

⚔️ TOP TOP LANE MATCHUPS (Min 2 games)
--------------------------------------------------------------------------------
Champion        vs                 | Games   | Win Rate
Poppy           vs K'Sante         | 2 games | 100.0% WR
Rek'Sai         vs Renekton        | 2 games | 100.0% WR
Rumble          vs K'Sante         | 5 games | 100.0% WR
Sion            vs K'Sante         | 2 games | 100.0% WR
Sion            vs Ambessa         | 5 games | 100.0% WR
Rumble          vs Sion            | 2 games | 100.0% WR
Galio           vs Rumble          | 3 games | 100.0% WR
Ambessa         vs Rumble          | 5 games | 80.0% WR
K'Sante         vs Mordekaiser     | 3 games | 66.7% WR
Rek'Sai         vs K'Sante         | 3 games | 66.7% WR
Ornn            vs Rumble          | 5 games | 60.0% WR
Renekton        vs K'Sante         | 5 games | 60.0% WR
Sion            vs Rek'Sai         | 7 games | 57.1% WR
Aatrox          vs Renekton        | 2 games | 50.0% WR
Ambessa         vs Rek'Sai         | 2 games | 50.0% WR

⚔️ TOP JUNGLE LANE MATCHUPS (Min 2 games)
--------------------------------------------------------------------------------
Champion        vs                 | Games   | Win Rate
Xin Zhao        vs Pantheon        | 2 games | 100.0% WR
Trundle         vs Qiyana          | 2 games | 100.0% WR
Dr. Mundo       vs Sejuani         | 2 games | 100.0% WR
Wukong          vs Maokai          | 2 games | 100.0% WR
Qiyana          vs Vi              | 2 games | 100.0% WR
Wukong          vs Jarvan IV       | 4 games | 75.0% WR
Jarvan IV       vs Pantheon        | 4 games | 75.0% WR
Jarvan IV       vs Trundle         | 4 games | 75.0% WR
Xin Zhao        vs Wukong          | 10 games | 70.0% WR
Xin Zhao        vs Vi              | 3 games | 66.7% WR
Naafiri         vs Vi              | 3 games | 66.7% WR
Trundle         vs Vi              | 3 games | 66.7% WR
Trundle         vs Xin Zhao        | 3 games | 66.7% WR
Pantheon        vs Qiyana          | 3 games | 66.7% WR
Qiyana          vs Xin Zhao        | 5 games | 60.0% WR

⚔️ TOP MID LANE MATCHUPS (Min 2 games)
--------------------------------------------------------------------------------
Champion        vs                 | Games   | Win Rate
Orianna         vs Aurora          | 2 games | 100.0% WR
LeBlanc         vs Taliyah         | 3 games | 100.0% WR
Galio           vs Ryze            | 2 games | 100.0% WR
Aurora          vs Ryze            | 2 games | 100.0% WR
Aurora          vs Annie           | 3 games | 100.0% WR
Azir            vs Aurora          | 2 games | 100.0% WR
Orianna         vs Galio           | 3 games | 66.7% WR
Azir            vs Taliyah         | 3 games | 66.7% WR
Taliyah         vs Ryze            | 9 games | 66.7% WR
Orianna         vs Akali           | 5 games | 60.0% WR
Orianna         vs Azir            | 7 games | 57.1% WR
Aurora          vs Taliyah         | 4 games | 50.0% WR
Syndra          vs Viktor          | 2 games | 50.0% WR
Anivia          vs Cassiopeia      | 2 games | 50.0% WR
Cassiopeia      vs Anivia          | 2 games | 50.0% WR
