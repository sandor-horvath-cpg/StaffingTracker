# StaffingTracker

todo: 
  - frontend: /all-candidate-data: switch label 'id' to 'position'
  - StatusEntity: change categories from(CG interview scheduled, Qualfied No GO) 
      Nov27: to (new entry(default), HR interview, professional interview, client interview)
      Nov28: to (GO, No-GO, Selected by Client), or to the 18 status from the received excel
  - change EmployeeShortCodeEntity to UserEntity
      add fields: code, role(e.g. Process Owner), name, email
  - add Spring Security
      based on UserEntity (implement this only after UserEntity is implemented)
      frontend: show logged in User Role (maybe name too)
  - implement CRUD for other entities(Client, Source, Position, User)
      frontend: add CRUD buttons/options
  - ApplicantEntity: add field: 'HR Owner': autofill when HR adds the applicant
      email notification to: 'HR Owner' and 'Process Owner'
      with subject containing: applicant [name] [source] [position] [status] [interview date]
  - new entity: ToDoEntity, with categories:
      •	Szakmai interjú
      •	HR interjú
      •	CV Capgemini formátummá alakítása
      •	További információ, akkor kell egy megjegyzés mező
      •	Más a process owner, megjegyzés mező
      (sidenote: some points here seems a bit redundant with the 18 status from the received excel)

todo (only after the above todos are finished):
  - külső interjúkat is nyomon követni (ez a belső intejúk után szokott lenni)
  - report generálás
  
done:
- db id: check if id is generated, if not add this
  
  
Business requirements
  menu
    Staffing request: consult with HR about requirements
    Tender: consult with HR about requirements
    Interview: consult with HR about requirements (the whole interview process will be needed probably)
  entities
    applicant: to track only the new, non-Capgemini applicants
      cvUploadPortal: needs to be String to show URL
  validation: not needed for now
