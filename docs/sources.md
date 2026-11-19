# Source registry

Teman only makes a medical or financial statement when it can point to one of these sources. Each content card in the app stores a `sourceID`, the exact URL, and a `lastReviewed` date. If a card is more than 120 days past review, the app marks it "may be out of date". This matters most for financial cards: MOH updates the Cancer Drug List every four months.

**Policy**
- **Tier 1, Singapore public bodies and national centres:** MOH, HealthHub, HSA, PDPC, NCCS, NCIS and the healthcare clusters. These are the default for medical and financial facts.
- **Tier 2, established Singapore charities:** SCS, BCF, CCF, the Singapore Hospice Council and HCA. These are the default for support services, and for practical coping when they agree with Tier 1.
- **Tier 3, international references:** NCI (cancer.gov) and similar. Teman uses these only for general definitions where no Tier 1 or 2 source exists, and labels them "International source".
- **Not used:** forums, blogs, insurer marketing, or personal sites. Some search results pointed to a personal GitHub page that lists Singapore helpline numbers. Teman does not use it.
- **Contact numbers** are verified by hand against the organisation's own contact page before each release. Several sources disagreed during research.

## Tier 1: government and national cancer centres

| ID | Source | Used for |
|---|---|---|
| `moh-cdl` | MOH, [Cancer Drug List](https://www.moh.gov.sg/managing-expenses/schemes-and-subsidies/medishield-life/cancer-drug-list/) | Explaining that MediShield Life and MediSave cover only outpatient cancer drugs on the list, that each drug has its own claim limits, and that the list is updated every four months |
| `moh-cds-limit` | MOH, [Higher MediShield Life claim limit for cancer drug services](https://www.moh.gov.sg/newsroom/higher-medishield-life-claim-limit-for-cancer-drug-services/) | The cancer drug services claim limit, which is separate from the drug limits |
| `moh-msl` | MOH, [MediShield Life benefits](https://www.moh.gov.sg/managing-expenses/schemes-and-subsidies/medishield-life/medishield-life-benefits/) | General MediShield Life coverage |
| `moh-no-denial` | MOH, [No one will be denied appropriate cancer care due to an inability to pay](https://www.moh.gov.sg/newsroom/no-one-will-be-denied-appropriate-cancer-care-due-to-an-inability-to-pay/) | Reassurance plus a route to a Medical Social Worker |
| `moh-hcg` | MOH, [Home Caregiving Grant](https://www.moh.gov.sg/newsroom/new-home-caregiving-grant-and-shorter-activation-time-for-respite-care-to-support-caregiving-in-the-community/) | Caregiver financial support. Amounts change, so Teman links to AIC for current figures |
| `cpf-msl` | CPF, [What MediShield Life covers you for](https://cpf.gov.sg/member/healthcare-financing/medishield-life/what-medishield-life-covers-you-for) | Plain-language MediShield Life explainer |
| `healthhub` | Synapxe and MOH, [HealthHub](https://synapxe.sg/healthtech/national-programmes/healthhub) | Telling patients where their official records, appointments and caregiver access live. Teman links out to it and does not duplicate it |
| `hsa-samd` | HSA, [Risk classification of SaMD and qualification of CDSS](https://www.hsa.gov.sg/announcements/regulatory-updates/update-for-guidelines-on-risk-classification-of-samd-and-qualification-of-clinical-decision-support-software-(cdss)) | Regulatory positioning (see safety doc) |
| `pdpc-health` | PDPC, [Advisory Guidelines for the Healthcare Sector](https://www.pdpc.gov.sg/organisations/regulations-decisions/regulatory-guidance/advisory-guidelines-for-the-healthcare-sector) | Privacy design |
| `nccs-first-visit` | NCCS, [Questions a cancer patient should ask at their first clinic appointment](https://www.nccs.com.sg/patient-care/questions-a-cancer-patient-should-ask-at-their-first-clinic-appointment) | Seed questions for the Ask module |
| `nccs-talking` | NCCS, [Talking to the doctor](https://www.nccs.com.sg/your-care/caregiver-support/talking-to-the-doctor) | Visit tips: say up front that you have questions, and write the answers down |
| `nccs-oncologist` | NCCS *In Good Health*, [Tell your oncologist what's important to you](https://www.nccs.com.sg/about-nccs/news/publications/in-good-health/issue-10/tell-your-oncologist-what-s-important-to-you) | The "What matters to me" card |
| `nccs-chemo-se` | NCCS, [Chemotherapy side effects](https://www.nccs.com.sg/your-care/patient-support/chemotherapy-side-effects) | Side-effect library |
| `nccs-pso` | NCCS, [Psychosocial Oncology](https://www.nccs.com.sg/our-specialties/psychosocial-oncology) | Emotional support: counselling, art therapy and support groups. No doctor's referral is needed |
| `nccs-psp` | NCCS, [Patient Support Programmes](https://www.nccs.com.sg/our-specialties/psychosocial-oncology/patient-support-programmes) | Support groups, talks and workshops |
| `nccs-psy-needs` | NCCS, [The top psychosocial needs of cancer patients](https://www.nccs.com.sg/patient-care/the-top-psychosocial-needs-of-cancer-patients) | The emotional check-in prompts |
| `nccs-pay` | NCCS, [MediSave, MediShield Life, MediFund](https://www.nccs.com.sg/clinic-visit/charges-and-payment/medisave-medishield-life-medifund) | MediFund eligibility, such as citizens and subsidised patients |
| `nccs-visit` | NCCS, [Visitor information](https://nccs.com.sg/patient-care/visitor-information) | Getting there: Outram Park MRT Exit 7 and the link bridge |
| `nccs-home-pc` | NCCS, [Call for earlier home palliative care](https://www.nccs.com.sg/news/patient-care/call-for-earlier-home-palliative-care-for-terminally-ill-patients) | Why to ask about palliative care early |
| `ncis-chemo-se` | NCIS, [Chemotherapy side effects](https://www.ncis.com.sg/cancer-information/chemotherapy/chemotherapy-side-effects) | Side-effect library, as a second national source |
| `ncis-pso` | NCIS, [Psychosocial Oncology](https://ncis.com.sg/our-services/specialties/psychosocial-oncology) | Emotional support at NUHS |
| `ncis-living` | NCIS, [Living with cancer](https://www.ncis.com.sg/our-services/living-with-cancer) | Support groups and survivorship |
| `sgh-shuttle` | SGH, [Wheelchair shuttle service](https://www.sgh.com.sg/patient-care/visitor-information/wheelchair-shuttle-service) | Getting there with a wheelchair, on the Outram campus |
| `nuhs-app` | NUHS, [NUHS App FAQ](https://nuhs.edu.sg/patient-care/nuhs-app/frequently-asked-questions) | Where NCIS patients see their appointments |
| `hx-chemo-1` | SingHealth HealthXchange, [Coping with chemotherapy side effects: infection, joint pain, sore mouth](https://www.healthxchange.sg/cancer/coping-tips/coping-chemotherapy-side-effects-infection-joint-pain-sore-mouth) | Side-effect coping tips |
| `hx-chemo-2` | SingHealth HealthXchange, [Coping with nausea, hair loss and bleeding](https://www.healthxchange.sg/cancer/coping-tips/cope-chemotherapy-side-effects-nausea-hair-loss-bleeding) | Side-effect coping tips |

## Tier 2: Singapore charities and care organisations

| ID | Source | Used for |
|---|---|---|
| `scs-understand` | Singapore Cancer Society, [Understanding your diagnosis and treatment](https://singaporecancersociety.org.sg/understanding-your-diagnosis-treatment/) | Diagnosis explainer, and questions to ask about recommended treatment, benefits and risks |
| `scs-guide` | SCS, [Your Guide to Cancer Care (PDF)](https://singaporecancersociety.org.sg/wp-content/uploads/2026/06/Your-Guide-to-Cancer-Care_English.pdf) | Navigation of the healthcare system |
| `scs-transport` | SCS, [Hospital transportation assistance](https://singaporecancersociety.org.sg/hospital-transportation-assistance/) | Home-to-hospital transport for chemotherapy and radiotherapy (citizens and PRs, means-tested) |
| `scs-finance` | SCS, [Financial assistance](https://singaporecancersociety.org.sg/?p=8930) | The Cancer Care Fund, Cancer Treatment Fund and Welfare Aid Fund |
| `scs-psych` | SCS, [Psychosocial support](https://singaporecancersociety.org.sg/?p=9451) | Counselling and support groups |
| `scs-contact` | SCS, [Connect with us](https://singaporecancersociety.org.sg/connect-with-us/) | The helpline number, verified before each release |
| `bcf` | [Breast Cancer Foundation](https://www.bcf.org.sg) | Befrienders, support groups, and wig and prosthesis support |
| `ccf` | [Children's Cancer Foundation](https://www.ccf.org.sg) | Children and families, PALS (schooling support), and bereavement |
| `shc` | [Singapore Hospice Council](https://singaporehospice.org.sg/) | Palliative and hospice care directory, and the common referral form |
| `365cps` | 365 Cancer Prevention Society, [Questions to ask your oncologist](https://365cps.org.sg/resourcehub/questions-to-ask-oncologist-treatment/) | More treatment questions, cross-checked against NCCS |

## Tier 3: international (definitions only)

| ID | Source | Used for |
|---|---|---|
| `nci-dict` | US National Cancer Institute, [NCI Dictionary of Cancer Terms](https://www.cancer.gov/publications/dictionaries/cancer-terms) | Plain definitions of terms that no Singapore glossary covers |
| `nci-questions` | NCI, [Questions to ask your doctor about your diagnosis](https://www.cancer.gov/about-cancer/diagnosis-staging/questions) | Staging question patterns |

## Contact numbers (verify before release)

These come from each organisation's own page, checked in November 2026. The app shows them with a "last verified" date.

| Service | Number | Source |
|---|---|---|
| Emergency ambulance | 995 | SCDF |
| NCCS Cancer Helpline | +65 6225 5655 | [NCCS](https://www.nccs.com.sg/contact-us) |
| NCCS Psychosocial Oncology | 6306 1777 | [NCCS](https://www.nccs.com.sg/our-specialties/psychosocial-oncology) |
| SCS general line | 1800-727-3333 | [SCS](https://singaporecancersociety.org.sg/connect-with-us/) |
| Agency for Integrated Care | 1800 650 6060 | AIC |
