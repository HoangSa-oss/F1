Cài đặt
    Sau khi git clone
    Vào Mongodb tạo database có tên là "f1" với cái collection có tên giống các file trong folder dbs
    Import data vào từng collection
    Vào Terminal chạy lệnh "npm i"
    Sau đó chạy lệnh lệnh "npm start"
Sử dụng     
    đường dẫn "http://localhost:3000/dhl/search"
        dùng để search cái thông tin DHL FASTEST LAP AWARD
        cú pháp data : 
            {
                "year":[2000,2010,"allYears"],
                "skip":option,
                "limit":option
            }
            tìm kiếm thông tin theo năm từ 2023 đến 1998 nếu xuất hiện "allYears" sẽ tìm tất cả các năm
    đường dẫn "http://localhost:3000/teams/search"
        dùng để search cái thông tin DHL FASTEST LAP AWARD
        cú pháp data : 
            {
                "teams":["Alfa Romeo Ferrari","Haas Ferrari","allTeams"],
                "year":[2010,2023, "allYears"],
                "skip":option,
                "limit":option
                }
            tìm kiếm thông tin theo năm từ 2023 đến 1998 và thông tin các teams
            nếu trong year xuất hiện "allYears" sẽ tìm tất cả các năm
            nếu trong teams xuất hiện "allTeams" sẽ tìm kiếm thông tin tổng hợp theo năm 

     đường dẫn "http://localhost:3000/races/search"
        dùng để search cái thông tin DHL FASTEST LAP AWARD
        cú pháp data : 
            {
                "country":["Bahrain","allRaces"],
                "year":[2010,2023,"allYears"],
                "skip":option,
                "limit":option
            }
             tìm kiếm thông tin theo năm từ 2023 đến 1998 và thông tin các races 
            nếu trong year xuất hiện "allYears" sẽ tìm tất cả các năm
            nếu trong teams xuất hiện "allRaces" sẽ tìm kiếm thông tin tổng hợp theo năm 

    đường dẫn "http://localhost:3000/drivers/search"
        dùng để search cái thông tin DHL FASTEST LAP AWARD
        cú pháp data : 
            {
                "teams":["Alfa Romeo Ferrari","Haas Ferrari","allDrivers"],
                "year":[2010,2023, "allYears"],
                "skip":option,
                "limit":option
                }
            tìm kiếm thông tin theo năm từ 2023 đến 1998 và thông tin các teams
            nếu trong year xuất hiện "allYears" sẽ tìm tất cả các năm
            nếu trong teams xuất hiện "allDrivers" sẽ tìm kiếm thông tin tổng hợp theo năm 

   

