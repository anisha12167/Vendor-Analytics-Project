#  Project Structure
66	+
67	+
```
66	68	
Vendor-Analytics-Project/
67	69	
│
68		-
├──
69		-
notebooks/
70		-
│ ├── Exploratory Data Analysis.ipynb
71		-
│ └── Vendor Performance Analysis.ipynb
70	+
├── notebooks/                 # Jupyter notebooks for analysis
71	+
│   ├── Exploratory Data Analysis.ipynb
72	+
│   └── Vendor Performance Analysis.ipynb
72	73	
│
73		-
├──
74		-
scripts/
75		-
│ ├── ingestion_db.py
76		-
│ └── get_vendor_summary.py
74	+
├── scripts/                   # Data ingestion & processing scripts
75	+
│   ├── ingestion_db.py
76	+
│   └── get_vendor_summary.py
77	77	
│
78		-
├── 
79		-
dashboard/
80		-
│ └── vendor_performance.pbix
78	+
├── dashboard/                 # Power BI dashboard
79	+
│   └── vendor_performance.pbix
81	80	
│
82		-
├── 
83		-
README.md
84		-
└── requirements.txt
81	+
├── README.md                  # Project documentation
82	+
└── requirements.txt           # Python dependencies
83	+
```
85	84	

86	85	

87	86	
---
