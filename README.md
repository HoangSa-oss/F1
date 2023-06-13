*Cài đặt

        Sau khi git clone

        Vào Mongodb tạo database có tên là "f1" với các collection có tên giống các file trong folder dbs

        Import data vào từng collection

        Vào Terminal chạy lệnh "npm i"

        Sau đó chạy lệnh lệnh "npm start"

*Sử dụng     

    **đường dẫn "http://localhost:3000/dhl/search" dùng để search các thông tin DHL FASTEST LAP AWARD
    .Cú pháp data : 

            {
            "year":[2000,2010,"allYears"],
            "skip":option,
            "limit":option
            }
    tìm kiếm thông tin theo năm từ 2023 đến 1998 nếu xuất hiện "allYears" sẽ tìm tất cả các năm

    **đường dẫn "http://localhost:3000/teams/search" dùng để search cái thông tin các team

    Cú pháp data : 

            {
            "teams":["Alfa Romeo Ferrari","Haas Ferrari","allTeams"],
            "year":[2010,2023, "allYears"],
            "skip":option,
            "limit":option
            }

    tìm kiếm thông tin theo năm từ 2023 đến 1998 và thông tin các teams
    .Nếu trong year xuất hiện "allYears" sẽ tìm tất cả các năm
    .Nếu trong teams xuất hiện "allTeams" sẽ tìm kiếm thông tin tổng hợp theo năm 

    **đường dẫn "http://localhost:3000/races/search"
    .dùng để search cái thông tin các races

    Cú pháp data : 

            {
            "country":["Bahrain","allRaces"],
            "year":[2010,2023,"allYears"],
            "skip":option,
            "limit":option
            }

    tìm kiếm thông tin theo năm từ 2023 đến 1998 và thông tin các races 
    .Nếu trong year xuất hiện "allYears" sẽ tìm tất cả các năm
    .Nếu trong teams xuất hiện "allRaces" sẽ tìm kiếm thông tin tổng hợp theo năm 

    **đường dẫn "http://localhost:3000/drivers/search"
    .dùng để search cái thông tin các drivers

    Cú pháp data : 

            {
            "teams":["Alfa Romeo Ferrari","Haas Ferrari","allDrivers"],
            "year":[2010,2023, "allYears"],
            "skip":option,
            "limit":option
            }

    tìm kiếm thông tin theo năm từ 2023 đến 1998 và thông tin các drivers
    .Nếu trong year xuất hiện "allYears" sẽ tìm tất cả các năm
    Nếu trong teams xuất hiện "allDrivers" sẽ tìm kiếm thông tin tổng hợp theo năm 

**các thông tin crawling được

let country =  [
    Bahrain
    Saudi Arabia
    Australia
    Azerbaijan
    Miami
    Emilia Romagna
    Monaco
    Spain
    Canada
    Austria
    Great Britain
    Hungary
    Belgium
    Netherlands
    Italy
    Singapore
    Japan
    Qatar
    United States
    Mexico
    Brazil
    Las Vegas
    Abu Dhabi
    France
    Portugal
    Styria
    Russia
    Turkey
    70th Anniversary
    Tuscany
    Eifel
    Sakhir
    China
    Germany
    Malaysia
    Europe
    South Korea
    India
    San Marino
    Argentina
    Luxembourg
]

let drivers = [
    Alexander Albon
    Fernando Alonso
    Valtteri Bottas
    Nyck De Vries
    Pierre Gasly
    Lewis Hamilton
    Nico Hulkenberg
    Charles Leclerc
    Kevin Magnussen
    Lando Norris
    Esteban Ocon
    Sergio Perez
    Oscar Piastri
    George Russell
    Carlos Sainz
    Logan Sargeant
    Lance Stroll
    Yuki Tsunoda
    Max Verstappen
    Guanyu Zhou
    Nicholas Latifi
    Daniel Ricciardo
    Mick Schumacher
    Sebastian Vettel
    Antonio Giovinazzi
    Robert Kubica
    Nikita Mazepin
    Kimi Räikkönen
    Jack Aitken
    Pietro Fittipaldi
    Romain Grosjean
    Daniil Kvyat
    Marcus Ericsson
    Brendon Hartley
    Sergey Sirotkin
    Stoffel Vandoorne
    Felipe Massa
    Jolyon Palmer
    Pascal Wehrlein
    Jenson Button
    Esteban Gutierrez 
    Rio Haryanto
    Felipe Nasr
    Nico Rosberg
    Pastor Maldonado
    Roberto Merhi
    Alexander Rossi
    Will Stevens
    Jules Bianchi
    Max Chilton
    Kamui Kobayashi
    Adrian Sutil
    Jean-Eric Vergne
    Paul di Resta
    Heikki Kovalainen
    Charles Pic
    Giedo van der Garde
    Mark Webber
    Jerome d'Ambrosio
    Pedro de la Rosa
    Timo Glock
    Narain Karthikeyan
    Vitaly Petrov
    Michael Schumacher
    Bruno Senna
    Jaime Alguersuari
    Rubens Barrichello
    Sebastien Buemi
    Karun Chandhok
    Nick Heidfeld
    Vitantonio Liuzzi
    Jarno Trulli
    Lucas di Grassi
    Christian Klien
    Sakon Yamamoto
    Luca Badoer
    Sebastien Bourdais
    Giancarlo Fisichella
    Kazuki Nakajima
    Nelson Piquet
    David Coulthard
    Anthony Davidson
    Takuma Sato
    Christijan Albers
    Ralf Schumacher
    Scott Speed
    Alexander Wurz
    Robert Doornbos
    Yuji Ide
    Franck Montagny
    Tiago Monteiro
    Juan Pablo Montoya
    Jacques Villeneuve
    Patrick Friesacher 
    Antonio Pizzonia
    Zsolt Baumgartner
    Gianmaria Bruni
    Cristiano da Matta
    Marc Gene
    Olivier Panis
    Giorgio Pantano
    Ricardo Zonta
    Ralph Firman
    Heinz-Harald Frentzen
    Nicolas Kiesa
    Jos Verstappen
    Justin Wilson
    Enrique Bernoldi
    Eddie Irvine
    Allan McNish
    Mika Salo
    Alex Yoong
    Jean Alesi
    Mika Hakkinen
    Luciano Burti
    Pedro Diniz
    Johnny Herbert
    Gaston Mazzacane
    Damon Hill
    Jan Magnussen
    Shinji Nakano
    Ricardo Rosset
    Toranosuke Takagi
    Esteban Tuero
    Gerhard Berger
    Nicola Larini
]

let teams = [
    nameTeam
    Alfa Romeo Ferrari
    AlphaTauri Honda RBPT
    Alpine Renault
    Aston Martin Aramco Mercedes
    Ferrari
    Haas Ferrari
    McLaren Mercedes
    Mercedes
    Red Bull Racing Honda RBPT
    Williams Mercedes
    AlphaTauri RBPT
    Red Bull Racing RBPT
    Alfa Romeo Racing Ferrari
    AlphaTauri Honda
    Aston Martin Mercedes
    Red Bull Racing Honda
    McLaren Renault
    Racing Point BWT Mercedes
    Renault
    Scuderia Toro Rosso Honda
    Force India Mercedes
    Force India Sahara
    Red Bull Racing TAG Heuer
    Sauber Ferrari
    McLaren Honda
    Toro Rosso
    MRT Mercedes
    Toro Rosso Ferrari
    Lotus Mercedes
    Marussia Ferrari
    Red Bull Racing Renault
    STR Renault
    Caterham Renault
    Lotus Renault
    Marussia Cosworth
    STR Ferrari
    Williams Renault
    HRT Cosworth
    Virgin Cosworth
    Williams Cosworth
    Lotus Cosworth
    RBR Renault
    Brawn Mercedes
    Sauber BMW
    Toyota
    Williams Toyota
    Force India Ferrari
    Honda
    Red Bull Renault
    Super Aguri Honda
    Spyker Ferrari
    MF1 Toyota
    RBR Ferrari
    STR Cosworth
    BAR Honda
    Jordan Toyota
    Minardi Cosworth
    RBR Cosworth
    Sauber Petronas
    Williams BMW
    Jaguar Cosworth
    Jordan Ford
    Arrows Cosworth
    Jordan Honda
    Minardi Asiatech
    Arrows Asiatech
    Benetton Renault
    Prost Acer
    Arrows Supertec
    Benetton Playlife
    Jordan Mugen Honda
    Arrows
    Minardi Ford
    Prost Peugeot
    Stewart Ford
    Williams Supertec
    Williams Mecachrome
]
