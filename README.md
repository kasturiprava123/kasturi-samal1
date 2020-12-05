def retrieve():
    
    import csv
    count = "Event_Id"
    count = input("enter the Event_id you want to search:")
    csv_file = csv.reader(open("miki.csv","r"))
    for row in csv_file:
        if count == row[3]:
            print(row)
        
retrieve()
