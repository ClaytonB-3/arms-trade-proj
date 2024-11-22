# arms-trade-proj


# final_data
cleaned_transfer_data.csv
- Raw data categorized with category and sub-category

- 
annual_delivery_data.csv
- Raw data split out into one row per year of materials delivered. Assigns equal parts of delivery to each year where deliver occured. 


YYYYMMDDone_row_one_country_data.csv
Description: Each transaction has been split into two rows  so that each country in the transaction has a row where they are the primary country. For example for a transaction between the United States and India where the United States was the supplier there would be two rows, one with USA in the countyr and one with India in the country. The Country Role column indicates if the row represents a transaction where the primary country is the supplier or recipient. The transcation_id column indicates a generated id for the transaction so that the two rows that pair up to be a transaction have the same id. The rest of the columns indicate information about the transaction. 

### Columns
| **Column Name**                                   | **Description**                                                                                                     |
|---------------------------------------------------|---------------------------------------------------------------------------------------------------------------------|
| `transaction_id`                                  | Identifier for each transaction. There are two rows per transaction                                                                           |
| `Country`                                         | Name of the country in the role indicated in Country Role                                                           |
| `Country Role`                                    | Role of the country in the transaction (e.g., Supplier or Recipient).                                               |
| `Partner Country`                                 | Name of the country on the other side of the transaction.                                                           |
| `Year of order`                                   | The year in which the order was placed for the weapons or equipment.                                                |
| `Number ordered`                                  | Quantity of weapons or equipment ordered.                                                                           |
| `Weapon designation`                              | Name or designation of the weapon or equipment.                                                                     |
| `Weapon description`                              | Brief description of the weapon or equipment, including its type or purpose.                                        |
| `status`                                          | Status of the transaction (e.g., New, Second hand).                                                                 |
| `Comments`                                        | Additional information or notes regarding the transaction.                                                         |
| `SIPRI TIV per unit`                              | SIPRI (Stockholm International Peace Research Institute) trend indicator value for a single unit of the weapon/equipment. |
| `SIPRI TIV for total order`                       | Absolute Value Total SIPRI TIV for the entire order of weapons or equipment.                                     |
| `Category`                                        | General category of the weapon or equipment (e.g., Aircraft, Helicopters).                                          |
| `Sub-Category`                                    | Specific sub-category of the weapon or equipment (e.g., Fighter/Combat Aircraft, Transport/Utility Helicopters).    |
| `SIPRI TIV for total order - Pos_Neg`             | Total SIPRI TIV for the order of weapons or equipment, negative if the primary country is the recipient.            |
| `Country Code`                                    | ISO 3-letter country code for the supplier country.                                                                 |
| `Armed forces personnel (% of total labor force)` | Percentage of the country’s labor force employed in the armed forces.                                               |
| `Armed forces personnel, total`                  | Total number of armed forces personnel in the supplier country.                                                     |
| `Arms exports (SIPRI trend indicator values)`     | Total arms exports by the supplier country, measured using SIPRI's trend indicator values.                          |
| `Arms imports (SIPRI trend indicator values)`     | Total arms imports by the supplier country, measured using SIPRI's trend indicator values.                          |
| `Military expenditure (% of GDP)`                | Percentage of the supplier country’s GDP spent on military expenditure.                                             |
| `Military expenditure (% of general government expenditure)` | Percentage of the supplier country’s general government expenditure spent on the military.                          |
| `Military expenditure (current LCU)`             | Military expenditure by the supplier country, measured in the local currency unit (LCU).                            |
