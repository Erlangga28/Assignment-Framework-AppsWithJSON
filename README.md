# Assignment Framework Programming 5.2
# By Erlangga Wahyu Utomo (5025201118)

## The JSON

```
  {
    "Name": "AFC Bournemouth",
    "Manager": "Eddie Howe",
    "City": "AFC Bournemouth is a professional association football club based in Kings Park, Boscombe, a suburb of Bournemouth, Dorset, England. The club competes in the Premier League, the highest division of English club football. Formed in 1899 as Boscombe, the club adopted their current name in 1971. Nicknamed The, Bournemouth have played their home games at Dean Court since 1910. Their home colours are red and black striped shirts, with black shorts and socks, inspired by that of Italian club A.C. Milan.",
    "Stadium": "Dean Court",
    "Code": "BOU",
    "Image": "https://upload.wikimedia.org/wikipedia/hif/5/53/AFC_Bournemouth_%282013%29.png",
    "Latitude": 50.734497062,
    "Longitude": -1.836329988
  },
  {
    "Name": "Arsenal",
    "Manager": "Arsene Wenger",
    "City": "Arsenal Football Club is an English professional football club based in Islington, London. Arsenal plays in the Premier League, the top flight of English football. The club has won 13 league titles (including one unbeaten title), a record 14 FA Cups, two League Cups, 16 FA Community Shields, one European Cup Winners' Cup, and one Inter-Cities Fairs Cup. In terms of trophies won, it is the third-most successful club in English football.",
    "Stadium": "Emirates Stadium",
    "Code": "ARS",
    "Image": "https://upload.wikimedia.org/wikipedia/hif/8/82/Arsenal_FC.png",
    "Latitude": 51.5555,
    "Longitude": -0.1057
  },
  {
    "Name": "Burnley",
    "Manager": "Sean Dyche",
    "City": "Burnley Football Club is an English association football club based in Burnley, Lancashire, that competes in the EFL Championship, the second tier of English football, following relegation from the 2021–22 Premier League. Founded on 18 May 1882, it was one of the first to become professional (in 1883), and subsequently put pressure on the Football Association to permit payments to players. The club entered the FA Cup for the first time in 1885–86 and was one of the 12 founder members of the Football League in 1888–89. From the 1950s until the 1970s, under chairman Bob Lord, the club became renowned for its youth policy and scouting system, and was one of the first to set up a purpose-built training ground. ",
    "Stadium": "Turf Moor",
    "Code": "BUR",
    "Image": "https://upload.wikimedia.org/wikipedia/it/7/76/FC_Burnley.png",
    "Latitude": 53.789167,
    "Longitude": -2.230278
  },
  {
  ...
  ```
  
  > The Connection 
  ```
  //Online
        var response = await httpClient.GetAsync("https://raw.githubusercontent.com/Erlangga28/Assignment-Framework-AppsWithJSON/main/EplTeams/MonkeyFinder/Resources/Raw/EplData.json");
        if (response.IsSuccessStatusCode)
        {
            monkeyList = await response.Content.ReadFromJsonAsync<List<Monkey>>();
        } 
  ```
  
  > The Color
  ```
  <Color x:Key="Primary">#e90052</Color>
            <Color x:Key="PrimaryDark">#FFA000</Color>
            <Color x:Key="Accent"> 	#00ff85</Color>
            <Color x:Key="newDark">#38003c</Color>

            <Color x:Key="LightBackground">#FAF9F8</Color>
            <Color x:Key="DarkBackground">#38003c</Color>

            <Color x:Key="LabelText">#1f1f1f</Color>
            <Color x:Key="LabelTextDark">White</Color>

            <Color x:Key="CardBackground">white</Color>
            <Color x:Key="CardBackgroundDark">#38003c</Color>
  ```
  
  ## The Result
  ![Assignment_2](https://github.com/Erlangga28/Assignment-Framework-AppsWithJSON/blob/main/ImagesResult/Result.mp4)
