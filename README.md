# Related Guarantees
Extend the guarantees ocds extension to generate modified guarantees based on contract modifications

## Example
```
{
  contract : {
    guaranties : [
      {
        id : 2,
        relatedGuarantee : 1,
        value : {
          amount : 4500,
          currency : "MXN"
        }
      },
      {
        id : 1,
        type : "check",
        date : "2019-01-06T00:00:00", 
        obligations: "fulfillment",
        value : {
          amount : 3500,
          currency : "MXN"
        },
        guarantor : {
          name : "INAI",
          id   : "MX-RFC-INA1412132Z8",
          address : {
            countryName:"México",
            locality:"Coyoacán",
            postalCode:"74530",
            region:"Ciudad de México",
            streetAddress:"Insurgentes Sur 3111"
          },
          contactPoint : {
            email:"el.kid@inai.org.mx",
            name:"Arturo Córdova",
            url:"http://inai.org.mx"
          },
          identifier : {
            id:"INA1402082Z8",
            juridicalPersonhood:"legalPerson",
            legalName:"Instituto Nacional de Transparencia, Acceso a la Información Pública y Protección de Datos Personales",
            scheme:"MX-RFC"
          }
        }
        period : {
          durationInDays:0,
          endDate:"2019-09-09T00:00:00",
          maxExtentDate:"2019-09-09T00:00:00",
          startDate:"2019-09-09T00:00:00"
        }
      }
    ]
  }
}
```
