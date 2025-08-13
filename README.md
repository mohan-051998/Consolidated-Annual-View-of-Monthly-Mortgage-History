import pandas as pd
from io import StringIO

csv_data = """Patient_ID,Name,Age,Gender,Visit_Date,Diagnosis,Treatment,Doctor_Name,Room_Type,Bed_Available,Total_Charges
P001,Arun Kumar,35,M,2025-08-10,Fever,Paracetamol 500mg,Dr. Meena,General Ward,Yes,1500
P002,Sneha Rani,28,F,2025-08-11,Dengue,Doxycycline,Dr. Rajesh,ICU,No,8500
P003,Vikram Das,42,M,2025-08-12,Typhoid,Cefixime 200mg,Dr. Priya,Private Room,Yes,6200
P004,Latha Devi,30,F,2025-08-13,Fever,Ibuprofen 400mg,Dr. Meena,General Ward,Yes,1800
P005,Ravi Shankar,50,M,2025-08-13,Malaria,Artemisinin Combo,Dr. Rajesh,ICU,No,9200
"""

df = pd.read_csv(StringIO(csv_data))
df.head()

import pandas as pd
from io import StringIO

csv_data = """Name,Age,Disease,Tablets,Doctor_Name
Sneha Rani,28,Dengue,Doxycycline,Dr. Rajesh
Latha Devi,30,Fever,Ibuprofen 400mg,Dr. Meena
Arun Kumar,35,Fever,Paracetamol 500mg,Dr. Meena
Vikram Das,42,Typhoid,Cefixime 200mg,Dr. Priya
Ravi Shankar,50,Malaria,Artemisinin Combo,Dr. Rajesh
"""

df = pd.read_csv(StringIO(csv_data))
df.head()
