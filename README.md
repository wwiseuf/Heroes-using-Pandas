# Pandas-Challenge


HEROES OF PYMOLI HOMEWORK CHALLENGE 


Prjoect was created to evaluate player statistics for Heroes of Pymoli game


This project was used with python code in jypter notewook from the Anaconda platform.   Pulling csv file from resource folder


With Pandas in mind using the code was created to analyize data of players their demographics and purchasing habits.  

example : 




    TOP SPENDER SET AND DATA FRAME 


    # group by SN
big_spenders = purchase_data_df.groupby(["SN"])

    # Purchase Count
big_spendersCount = big_spenders["Item ID"].count()

    # Average Purchase Price
big_spenders_avg = big_spenders["Price"].mean()

    # Total Purchase Value 
big_spenders_total = big_spenders["Price"].sum()

    # Create DataFrame
big_spenders = pd.DataFrame({"Purchase Count" : big_spendersCount,
                             "Average Purchase Price" : big_spenders_avg,
                             "Total Purchase Value" : big_spenders_total
                            })

big_spenders = big_spenders.sort_values(['Total Purchase Value'],ascending=False)


    # Clean up style
big_spenders.head(5).style.format({"Average Purchase Price" : "${:,.2f}",
                         "Total Purchase Value" : "${:,.2f}",
                         })



using pandas in juypter simnply load the csv data from file location and run data




         




