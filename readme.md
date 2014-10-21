
## Payments API Documentation
-------------------------------------
* ### checkifdom:
This is used to check if the card no. is domestic or international.
--------



#### URL : [HOST] /common/checkifdom/

**Params**

Keys | Description | Sample Value
--- |---| ---
ccprefix |Card no. prefix| 429393


```Example JSON Response```

 

    {
        "isDomestic": "Y",
        "issuingBank": "KOTAK ",
        "cardType": "VISA",
        "cardCategory": "DC"
    }
                    

-------------------------------------
* checknbstatus:
    This is used to check if the net banking is up and working.
--------




#### URL : [HOST] /common/checknbstatus/

**Params**

Keys | Description | Sample Value
--- |---| ---
ibibo_code |Ibibo mapping to Bank code| 162B


```Example JSON Response```


    {
        "ibibo_code": "162B",
        "title": "Kotak Mahindra Bank",
        "up_status": 1
    }


-------------------------------------
* getemicharges:
    This is used to get emi charges for the entered amount.
--------



#### URL : [HOST] /common/getemicharges/

**Params**

Keys | Description | Sample Value
--- |---| ---
amount |The amount for which emi is to be calculated| 9649


```Example JSON Response```

         
        {
            "20": {
                "EMI03": {
                    "emiBankInterest": "12",
                    "bankRate": null,
                    "bankCharge": 0,
                    "amount": 3216.33,
                    "emi_value": 3280.87,
                    "emi_interest_paid": 193.61
                },
                "EMI06": {
                    "emiBankInterest": "12",
                    "bankRate": null,
                    "bankCharge": 0,
                    "amount": 1608.17,
                    "emi_value": 1664.92,
                    "emi_interest_paid": 340.52
                }
            }
        }
                    
	

-------------------------------------
* getpayuobject:

--------

#### URL : [HOST] /common/getpayuobject/

**Params**

Keys | Description | Sample Value
--- |---| ---
go_pay_pg | Payment Gateway | citrus


```Example JSON Response```

         
        {
            "emi": {
                "EMI03": {
                    "bank": "CITI",
                    "title": "3 Months",
                    "pgId": "20",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "EMI06": {
                    "bank": "CITI",
                    "title": "6 Months",
                    "pgId": "20",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "100"
                }
            },
            "netbanking": {
                "ALLB": {
                    "title": "Allahabad Bank NetBanking",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "6"
                },
                "ADBB": {
                    "title": "Andhra Bank",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "7"
                },
                "AXIB": {
                    "title": "AXIS Bank NetBanking",
                    "pgId": "23",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "1"
                },
                "BBKB": {
                    "title": "Bank of Bahrain and Kuwait",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "8"
                },
                "BBCB": {
                    "title": "Bank of Baroda - Corporate Banking",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "9"
                },
                "BBRB": {
                    "title": "Bank of Baroda - Retail Banking",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "10"
                },
                "BOIB": {
                    "title": "Bank of India",
                    "pgId": "53",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "11"
                },
                "BOMB": {
                    "title": "Bank of Maharashtra",
                    "pgId": "58",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "12"
                },
                "CABB": {
                    "title": "Canara Bank",
                    "pgId": "69",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "CSBN": {
                    "title": "Catholic Syrian Bank",
                    "pgId": "60",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "14"
                },
                "CBIB": {
                    "title": "Central Bank Of India",
                    "pgId": "68",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "CITNB": {
                    "title": "Citibank Netbanking",
                    "pgId": "20",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "5"
                },
                "CUBB": {
                    "title": "City Union Bank",
                    "pgId": "67",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "CRPB": {
                    "title": "Corporation Bank",
                    "pgId": "33",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "16"
                },
                "DSHB": {
                    "title": "Deutsche Bank",
                    "pgId": "64",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "DCBB": {
                    "title": "Development Credit Bank",
                    "pgId": "42",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "19"
                },
                "DLSB": {
                    "title": "Dhanlaxmi Bank",
                    "pgId": "89",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "58"
                },
                "FEDB": {
                    "title": "Federal Bank",
                    "pgId": "59",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "21"
                },
                "HDFB": {
                    "title": "HDFC Bank",
                    "pgId": "56",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "2"
                },
                "ICIB": {
                    "title": "ICICI Netbanking",
                    "pgId": "19",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "3"
                },
                "IDBB": {
                    "title": "IDBI Bank",
                    "pgId": "32",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "25"
                },
                "INDB": {
                    "title": "Indian Bank ",
                    "pgId": "74",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "INOB": {
                    "title": "Indian Overseas Bank",
                    "pgId": "45",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "23"
                },
                "INIB": {
                    "title": "IndusInd Bank",
                    "pgId": "28",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "24"
                },
                "INGB": {
                    "title": "ING Vysya Bank",
                    "pgId": "75",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "28"
                },
                "JAKB": {
                    "title": "Jammu and Kashmir Bank",
                    "pgId": "37",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "27"
                },
                "KRKB": {
                    "title": "Karnataka Bank",
                    "pgId": "35",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "28"
                },
                "KRVB": {
                    "title": "Karur Vysya - Retail Netbanking",
                    "pgId": "71",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "162B": {
                    "title": "Kotak Mahindra Bank",
                    "pgId": "77",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "LVCB": {
                    "title": "Laxmi Vilas Bank-Corporate",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "32"
                },
                "LVRB": {
                    "title": "Laxmi Vilas Bank-Retail",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "33"
                },
                "OBCB": {
                    "title": "Oriental Bank of Commerce",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "34"
                },
                "CPNB": {
                    "title": "Punjab National Bank - Corporate Banking",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "35"
                },
                "PNBB": {
                    "title": "Punjab National Bank - Retail Banking",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "36"
                },
                "RTN": {
                    "title": "Ratnakar Bank ",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "37"
                },
                "SVCB": {
                    "title": "Shamrao Vitthal Co-operative Bank",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "39"
                },
                "SOIB": {
                    "title": "South Indian Bank",
                    "pgId": "36",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "40"
                },
                "SBBJB": {
                    "title": "State Bank of Bikaner and Jaipur",
                    "pgId": "46",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "42"
                },
                "SBHB": {
                    "title": "State Bank of Hyderabad",
                    "pgId": "47",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "43"
                },
                "SBIB": {
                    "title": "State Bank of India",
                    "pgId": "39",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "4"
                },
                "SBMB": {
                    "title": "State Bank of Mysore",
                    "pgId": "48",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "44"
                },
                "SBPB": {
                    "title": "State Bank of Patiala",
                    "pgId": "78",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "SBTB": {
                    "title": "State Bank of Travancore",
                    "pgId": "49",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "46"
                },
                "SYDB": {
                    "title": "Syndicate Bank",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "47"
                },
                "TMBB": {
                    "title": "Tamilnad Mercantile Bank",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "48"
                },
                "UCOB": {
                    "title": "UCO Bank",
                    "pgId": "1",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "49"
                },
                "UBIB": {
                    "title": "Union Bank - Retail Netbanking",
                    "pgId": "25",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "50"
                },
                "UNIB": {
                    "title": "United Bank Of India",
                    "pgId": "63",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "51"
                },
                "VJYB": {
                    "title": "Vijaya Bank",
                    "pgId": "70",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "YESB": {
                    "title": "Yes Bank",
                    "pgId": "26",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "53"
                }
            },
            "creditcard": {
                "AMEX": {
                    "title": "AMEX Cards",
                    "pgId": "54",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "CC": {
                    "title": "Credit Card",
                    "pgId": "38",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "DINR": {
                    "title": "Diners",
                    "pgId": "8",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "100"
                }
            },
            "debitcard": {
                "CITD": {
                    "title": "CITI Debit Card",
                    "pgId": "38",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "7"
                },
                "MAST": {
                    "title": "MasterCard Debit Cards (All Banks)",
                    "pgId": "8",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "2"
                },
                "MAES": {
                    "title": "Other Maestro Cards",
                    "pgId": "8",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "4"
                },
                "RUPAY": {
                    "title": "Rupay Debit Card",
                    "pgId": "98",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "100"
                },
                "SMAE": {
                    "title": "State Bank Maestro Cards",
                    "pgId": "38",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "3"
                },
                "VISA": {
                    "title": "Visa Debit Cards (All Banks)",
                    "pgId": "8",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "1"
                }
            },
            "cashcard": {
                "CPMC": {
                    "title": "Citibank Reward Points",
                    "pgId": "20",
                    "show_form": "1",
                    "bank_id": null,
                    "pt_priority": "8"
                }
            },
            "paisawallet": {
                "PAYUW": {
                    "title": "Paisa Wallet non-ROD",
                    "pgId": "79",
                    "show_form": "0",
                    "bank_id": null,
                    "pt_priority": "100"
                }
            }
        }





## To implement Payment in Verticals

### To Integrate Payment part :

```  
(  Sample Implementation can be viewed from :
URL:    {{HOST}}/payments/dummy-payment )
```
---------------------------------------------

    
* On the page where you want show payment options do the following :
    
* Include the two files from goflight repository:
``` 
	1. payopts.html    ('/travelibibo/html/templates/v2/common/payopts.html')
	2. pDataForm.html  ( '/travelibibo/html/templates/v2/common/pDataForm.html')
        
```

* Hidden fields that must be present :
```
    $('#native_pay_amnt').val()   --The final amount that should be taken from payu.
    $('#hiddenudf2').val()        --(true/false) Whether user is logged in or not.
    $('#go_pay_pg').val()         --(payu/citrus/adyen) Which Payment gateway to use for taking the payment.
    
    $('#email').val()             --User email. 
    $('#mobile').val()            --User Mobile.
```
  
* Once the user clicks on 'Make Payment' 
```     
     Call the javascript function 'gi.payU.initDoc()' 
     This will load all payment options and its fields. 
```
All the hidden field values in pDataForm must be set as per the selected payment gateway.

Make Ajax Call to Submit.
On Success response
gi.payU.updateInitData(respData,true);
( for reference you can view the files :
/travelibibo/html/templates/v2/payments/dummy_payment.html
/travelibibo/payments/uat_views.py )


Javascript files to be included :
{% block postloadjs %}
    <script type="text/javascript" src="/js/v2/lib-combined-min-v2.js">
    {% if DEBUG %}
        
        type="text/javascript"></script>
        <script src="/js/v2/jquery.payment.js" type="text/javascript" ></script>
        <script src="/js/v2/go_rsa.js" type="text/javascript" ></script>
        <script src="/js/v2/sjcl.js" type="text/javascript" ></script>
        <script src="/js/v2/aes_key.js" type="text/javascript" ></script>
        <script src="/js/v2/go_payment.js" type="text/javascript" ></script>
        <script src="/js/v2/goibibo_booking.js" type="text/javascript" ></script>
    {% else %}
        <script src="/js/v2/combined-native-payment-min.js" type="text/javascript" ></script>
    {% endif %}
{% endblock %}

---------------------------------------------




###To integrate Payment in Mobile:

From the submit response set the value as per the payment gateway:

#### For citrus: 

Initialize the following dict object citrus_card_obj / citrus_netbank_obj :

```
    citrus_card_obj : {
    		"returnUrl":"",
    		"notifyUrl":"",
    		"amount": {"value": "", "currency": ""},
    		"merchantAccessKey": "",
    		"paymentToken": {
    			"type": "paymentOptionToken",
    			"paymentMode": {
    				"cvv": "",
    				"holder": "",
    				"number": "",
    				"scheme": "",
    				"type": "",
    				"expiry": ""
    			}
    		},
    		"merchantTxnId": "",
    		"requestSignature": "", 
    		"userDetails": {
    			"lastName": "",
    			"firstName": "",
    			"address": {
    				"state": "",
    				"street2": "",
    				"zip": "",
    				"street1": "",
    				"country": "India",
    				"city": ""
    			},
    			"email": "",
    			"mobileNo": ""
    		}
    	},
    	citrus_netbank_obj : {
    		"returnUrl":"",
    		"notifyUrl":"",
    		"amount": {"value": "", "currency": ""},
    		"merchantAccessKey": "",
    		"paymentToken": {
    			"type": "paymentOptionToken",
    			"paymentMode": {
    				"type": "netbanking",
    				"code": "",
    			}
    		},
    		"merchantTxnId": "",
    		"requestSignature": "", 
    		"userDetails": {
    			"lastName": "",
    			"firstName": "",
    			"address": {
    				"state": "",
    				"street2": "",
    				"zip": "",
    				"street1": "",
    				"country": "India",
    				"city": ""
    			},
    			"email": "",
    			"mobileNo": ""
    		}
    	}
	
```
###To initiate citrus session, make a JSON POST

URL: provided in the submit response

**Params**

Keys| Description|Sample Value
-----------------------|-----------------------|-----------------
citruspayObj.returnUrl                  |  |
citruspayObj.notifyUrl                  | |
citruspayObj.amount.value | |
citruspayObj.amount.currency |  | INR
citruspayObj.merchantAccessKey | | D2RT5WU6746IIIC4AWH8
citruspayObj.merchantTxnId || GOFLD684681410344086
citruspayObj.requestSignature | | 84e0849de841da0404a2cedc80d703cab4ff9920
citruspayObj.userDetails.firstName | | Tushar
citruspayObj.userDetails.lastName | | Kanti
citruspayObj.userDetails.email | | tushar.kanti@ibibogroup.com
citruspayObj.userDetails.mobileNo | | 8904718480
citruspayObj.userDetails.address.state | | 
citruspayObj.userDetails.address.city | |
citruspayObj.userDetails.address.country | |
citruspayObj.userDetails.address.zip | |
citruspayObj.userDetails.address.street1  | |
citruspayObj.userDetails.address.street2 | |


```Returns / Response:```

Keys | Description | Sample Value
---- | ----------- | ---------
resp.pgRespCode | returns 0 for successful transaction | 
resp.redirectUrl | After transaction the url to which it should be re-directed | 
    
Sample:
```
    {
        returnUrl : "http://goibibo.local:8000/payments/payment-success?s=citrus",
        notifyUrl : "http://goibibo.local:8000/bookingcall/?s=citrus",
        currency : "INR",
        orderAmount : "8173",
        merchantTxnId : "GOTEST274eb1413802864",
        sessionurl : "https://sandboxadmin.citruspay.com/service/moto/authorize/struct/payment",
        access_key : "D2RT5WU6746IIIC4AWH8",
        secSignature : "0102e5a171b84e14df36a72d5517f4b354f27dc4",
        txnid : "GOTEST274eb1413802864",
        merchantid : "2sybxc1c5z",
        purl : "https://sandbox.citruspay.com/2sybxc1c5z"
    }
```       
   
-   
    ###To initiate Adyen payments session:
    
    Initialize the following dict object:
    
    
```
    adyen_card_data : {
    			'generationtime':'',
    			'number':'',
    			'holderName': '',
    			'cvc':'',
    			'expiryMonth':'',
    			'expiryYear':'',
    	}
 ```
   
POST URL : {HOST}/payments/makepayment/

_Params_

Keys | Description | Sample Value
---- | ----------- | ---------
adyen-encrypted-data | |
amount | |
currency | |
shopperEmail | |
reference | | 
shopperReference | |
fraudOffset | |
merchantAccount | |
returnUrl | |
signature | |
    

```Returns / Response:```

Keys | Description | Sample Value
---- | ----------- | ---------
resp.status | Based on transaction its value is success/failed/tempered | success

Sample:
```
    {
        currency : "INR",
        amount : "8173",
        returnUrl : "http://goibibo.local:8000/payments/payment-success?s=adyen",
        reference : "GOTEST62aeb1413803169",
        shopperEmail : "tushar@gmail.com",
        shopperReference : "travel-DEL-BLR-20141008-0525",
        reqsignature : "a0a392d41f71220f7850a3df13a9e7dac7915f66d285b6ed01284a2d17134c931c564a1fb948d70770a4e29b7134a705ac47095bd907d160db2de55ffc6d7daa",
        fraudOffset : "0",
        merchantAccount : "IbiboCOM"
    }  
```
