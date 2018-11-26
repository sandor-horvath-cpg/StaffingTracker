# StaffingTracker

todo: 
  frontend: /all-candidate-data: switch label 'id' to 'position'
  db id: check if id is generated, if not add this
  add Spring security
    show User Role (maybe name too) (implement this only after UserEntity is implemented)
  implement CRUD for other entities(client, source, position, EmployeeShortCode)
  research: Devon email notification (for PO with interview date, etc)
  StatusEntity: change categories from(CG interview scheduled, Qualfied No GO) 
    to (new entry(default), HR interview, professional interview, client interview)
  Process Owner(EmployeeShortCodeEntity): add fields: name, email, beside the code
    upd: change this to UserEntity with code, role(e.g. PO), name, email

Business requirements
  menu
    Staffing request: consult with HR about requirements
    Tender: consult with HR about requirements
    Interview: consult with HR about requirements (the whole interview process will be needed probably)
  entities
    applicant: to track only the new, non-Capgemini applicants
      cvUploadPortal: needs to be String to show URL
  validation: not needed for now
