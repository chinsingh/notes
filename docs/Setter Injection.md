# Setter Injection

```abap
CLASS … DEFINITION … .
  PUBLIC SECTION.
    METHODS set_cash_provider IMPORTING i_cash_provider TYPE REF TO if_cash_provider.
  PRIVATE SECTION.
    DATA m_cash_provider TYPE REF TO if_cash_provider.
…
ENDCLASS.

CLASS … IMPLEMENTATION.
  METHOD set_cash_provider.
    m_cash_provider = i_cash_provider.
  ENDMETHOD.
…
ENDCLASS.
```
