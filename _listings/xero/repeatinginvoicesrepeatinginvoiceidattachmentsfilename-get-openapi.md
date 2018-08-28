---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Repeatinginvoices Repeatinginvoice Attachments Filename
  description: Get repeatinginvoices repeatinginvoice attachments filename.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountID}/Attachments/{FileName}:
    get:
      summary: Get Accounts Attachments Filename
      description: Get accounts account attachments filename.
      operationId: getAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-get
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
    post:
      summary: Post Accounts Attachments Filename
      description: Post accounts account attachments filename.
      operationId: postAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-post
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
  /BankTransactions/{BankTransactionID}/Attachments/{FileName}:
    get:
      summary: Get Bank Transactions Banktransaction Attachments Filename
      description: Get banktransactions banktransaction attachments filename.
      operationId: getBanktransactionsBanktransactionAttachmentsFilename
      x-api-path-slug: banktransactionsbanktransactionidattachmentsfilename-get
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
      - FileName
    post:
      summary: Post Bank Transactions Banktransaction Attachments Filename
      description: Post banktransactions banktransaction attachments filename.
      operationId: postBanktransactionsBanktransactionAttachmentsFilename
      x-api-path-slug: banktransactionsbanktransactionidattachmentsfilename-post
      parameters:
      - in: path
        name: BankTransactionID
        description: The Xero generated unique identifier for an bank transaction
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - BankTransactions
      - BankTransactionID
      - Attachments
      - FileName
  /BankTransfers/{BankTransferID}/Attachments/{FileName}:
    get:
      summary: Get Banks Transfers Attachments Filename
      description: Get banktransfers banktransfer attachments filename.
      operationId: getBanktransfersBanktransferAttachmentsFilename
      x-api-path-slug: banktransfersbanktransferidattachmentsfilename-get
      parameters:
      - in: path
        name: BankTransferID
        description: The Xero generated unique identifier for an BankTransfer
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
      - Attachments
      - FileName
    post:
      summary: Post Banks Transfers Attachments Filename
      description: Post banktransfers banktransfer attachments filename.
      operationId: postBanktransfersBanktransferAttachmentsFilename
      x-api-path-slug: banktransfersbanktransferidattachmentsfilename-post
      parameters:
      - in: path
        name: BankTransferID
        description: The Xero generated unique identifier for a BankTransfer
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - BankTransfers
      - BankTransferID
      - Attachments
      - FileName
  /Contacts/{ContactID}/Attachments/{FileName}:
    get:
      summary: Get Contacts Contact Attachments Filename
      description: Get contacts contact attachments filename.
      operationId: getContactsContactAttachmentsFilename
      x-api-path-slug: contactscontactidattachmentsfilename-get
      parameters:
      - in: path
        name: ContactID
        description: The Xero generated unique identifier for a Contact
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - ContactID
      - Attachments
      - FileName
    post:
      summary: Post Contacts Contact Attachments Filename
      description: Post contacts contact attachments filename.
      operationId: postContactsContactAttachmentsFilename
      x-api-path-slug: contactscontactidattachmentsfilename-post
      parameters:
      - in: path
        name: ContactID
        description: The Xero generated unique identifier for a Contact
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - ContactID
      - Attachments
      - FileName
  /CreditNotes/{CreditNoteID}/Attachments/{FileName}:
    get:
      summary: Get Creditnotes Creditnote Attachments Filename
      description: Get creditnotes creditnote attachments filename.
      operationId: getCreditnotesCreditnoteAttachmentsFilename
      x-api-path-slug: creditnotescreditnoteidattachmentsfilename-get
      parameters:
      - in: path
        name: CreditNoteID
        description: The Xero generated unique identifier for a CreditNote
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - CreditNotes
      - CreditNoteID
      - Attachments
      - FileName
    post:
      summary: Post Creditnotes Creditnote Attachments Filename
      description: Post creditnotes creditnote attachments filename.
      operationId: postCreditnotesCreditnoteAttachmentsFilename
      x-api-path-slug: creditnotescreditnoteidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: CreditNoteID
        description: The Xero generated unique identifier for a CreditNote
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - CreditNotes
      - CreditNoteID
      - Attachments
      - FileName
  /Invoices/{InvoiceID}/Attachments/{FileName}:
    get:
      summary: Get Invoices Invoice Attachments Filename
      description: Get invoices invoice attachments filename.
      operationId: getInvoicesInvoiceAttachmentsFilename
      x-api-path-slug: invoicesinvoiceidattachmentsfilename-get
      parameters:
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: path
        name: InvoiceID
        description: The Xero generated unique identifier for an Invoice
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Invoices
      - InvoiceID
      - Attachments
      - FileName
    post:
      summary: Post Invoices Invoice Attachments Filename
      description: Post invoices invoice attachments filename.
      operationId: postInvoicesInvoiceAttachmentsFilename
      x-api-path-slug: invoicesinvoiceidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      - in: path
        name: InvoiceID
        description: The Xero generated unique identifier for an Invoice
      responses:
        200:
          description: OK
      tags:
      - Invoices
      - InvoiceID
      - Attachments
      - FileName
  /ManualJournals/{ManualJournalID}/Attachments/{FileName}:
    get:
      summary: Get Manualjournals Manualjournal Attachments Filename
      description: Get manualjournals manualjournal attachments filename.
      operationId: getManualjournalsManualjournalAttachmentsFilename
      x-api-path-slug: manualjournalsmanualjournalidattachmentsfilename-get
      parameters:
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: path
        name: ManualJournalID
        description: The Xero generated unique identifier for a Manual Journal
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - ManualJournals
      - ManualJournalID
      - Attachments
      - FileName
    post:
      summary: Post Manualjournals Manualjournal Attachments Filename
      description: Post manualjournals manualjournal attachments filename.
      operationId: postManualjournalsManualjournalAttachmentsFilename
      x-api-path-slug: manualjournalsmanualjournalidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      - in: path
        name: ManualJournalID
        description: The Xero generated unique identifier for a Manual Journal
      responses:
        200:
          description: OK
      tags:
      - ManualJournals
      - ManualJournalID
      - Attachments
      - FileName
  /PurchaseOrders/{PurchaseOrderID}/Attachments/{FileName}:
    get:
      summary: Get Purchaseorders Purchaseorder Attachments Filename
      description: Get purchaseorders purchaseorder attachments filename.
      operationId: getPurchaseordersPurchaseorderAttachmentsFilename
      x-api-path-slug: purchaseorderspurchaseorderidattachmentsfilename-get
      parameters:
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      - in: path
        name: PurchaseOrderID
        description: The Xero generated unique identifier for a purchase order
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
      - Attachments
      - FileName
    post:
      summary: Post Purchaseorders Purchaseorder Attachments Filename
      description: Post purchaseorders purchaseorder attachments filename.
      operationId: postPurchaseordersPurchaseorderAttachmentsFilename
      x-api-path-slug: purchaseorderspurchaseorderidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      - in: path
        name: PurchaseOrderID
        description: The Xero generated unique identifier for a purchase order
      responses:
        200:
          description: OK
      tags:
      - PurchaseOrders
      - PurchaseOrderID
      - Attachments
      - FileName
  /Receipts/{ReceiptID}/Attachments/{FileName}:
    get:
      summary: Get Receipts Receipt Attachments Filename
      description: Get receipts receipt attachments filename.
      operationId: getReceiptsReceiptAttachmentsFilename
      x-api-path-slug: receiptsreceiptidattachmentsfilename-get
      parameters:
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      - in: path
        name: ReceiptID
        description: The Xero generated unique identifier for a Receipt
      responses:
        200:
          description: OK
      tags:
      - Receipts
      - ReceiptID
      - Attachments
      - FileName
    post:
      summary: Post Receipts Receipt Attachments Filename
      description: Post receipts receipt attachments filename.
      operationId: postReceiptsReceiptAttachmentsFilename
      x-api-path-slug: receiptsreceiptidattachmentsfilename-post
      parameters:
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      - in: path
        name: ReceiptID
        description: The Xero generated unique identifier for a Receipt
      responses:
        200:
          description: OK
      tags:
      - Receipts
      - ReceiptID
      - Attachments
      - FileName
  /RepeatingInvoices/{RepeatingInvoiceID}/Attachments/{FileName}:
    get:
      summary: Get Repeatinginvoices Repeatinginvoice Attachments Filename
      description: Get repeatinginvoices repeatinginvoice attachments filename.
      operationId: getRepeatinginvoicesRepeatinginvoiceAttachmentsFilename
      x-api-path-slug: repeatinginvoicesrepeatinginvoiceidattachmentsfilename-get
      parameters:
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      - in: path
        name: RepeatingInvoiceID
        description: The Xero generated unique identifier for a RepeatingInvoice
      responses:
        200:
          description: OK
      tags:
      - RepeatingInvoices
      - RepeatingInvoiceID
      - Attachments
      - FileName
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---