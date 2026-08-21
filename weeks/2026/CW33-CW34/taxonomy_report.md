**Taxonomy Report --- CW33 + CW34 2026**

**Report Metadata**

  ----------------------------------------------------------------------------------
  **Field**       **Value**
  --------------- ------------------------------------------------------------------
  Reporting       CW33 + CW34 2026
  period          

  Incident count  56

  Generated at    2026-08-21T05:01:00Z

  Orchestrator    v1.5
  version         

  incidents.csv   89A8F1937EC8A8A52F81BF27568ED95DA72C0BE1A1CFF35626BC09CD96DCFC59
  SHA-256         
  ----------------------------------------------------------------------------------

The supplied week-close metadata explicitly records 56 incidents and the
generation timestamp and orchestrator version. The supplied SHA-256
value also matches the attached incidents.csv byte-for-byte.

**Incident Type Distribution**

  ------------------------------------------
  **Incident     **Incidents**   **Share**
  Type**                         
  -------------- --------------- -----------
  scam           35              62.5%

  user_mistake   12              21.4%

  hack           9               16.1%

  Total          56              100.0%
  ------------------------------------------

Scams remain the dominant category, accounting for almost two-thirds of
all incidents. User mistakes represent slightly more than one-fifth,
while hacks account for approximately one-sixth.

**Full Taxonomy Distribution**

  ---------------------------------------------------------------------------------------
  **Incident     **Incident Subtype**         **Incidents**   **Share of All **Share
  Type**                                                      Incidents**    Within
                                                                             Type**
  -------------- ---------------------------- --------------- -------------- ------------
  scam           exchange_scam                17              30.4%          48.6%

  scam           social_engineering           10              17.9%          28.6%

  scam           job_scam                     2               3.6%           5.7%

  scam           phishing                     2               3.6%           5.7%

  scam           romance_scam                 2               3.6%           5.7%

  scam           airdrop_scam                 1               1.8%           2.9%

  scam           token_launch_scam            1               1.8%           2.9%

  hack           wallet_software_exploit      5               8.9%           55.6%

  hack           social_engineering_hack      2               3.6%           22.2%

  hack           fake_app_or_extension_hack   1               1.8%           11.1%

  hack           spyware                      1               1.8%           11.1%

  user_mistake   wrong_network                6               10.7%          50.0%

  user_mistake   lost_wallet_access           3               5.4%           25.0%

  user_mistake   wrong_address                2               3.6%           16.7%

  user_mistake   seed_phrase_exposure         1               1.8%           8.3%

  Total                                       56              100.0%         
  ---------------------------------------------------------------------------------------

**Scam Taxonomy**

  ---------------------------------------------------------------------
  **Scam Subtype**     **Incidents**   **Share of    **Share of All
                                       Scams**       Incidents**
  -------------------- --------------- ------------- ------------------
  exchange_scam        17              48.6%         30.4%

  social_engineering   10              28.6%         17.9%

  job_scam             2               5.7%          3.6%

  phishing             2               5.7%          3.6%

  romance_scam         2               5.7%          3.6%

  airdrop_scam         1               2.9%          1.8%

  token_launch_scam    1               2.9%          1.8%

  Total                35              100.0%        62.5%
  ---------------------------------------------------------------------

The scam taxonomy is strongly concentrated. exchange_scam and
social_engineering together account for 27 of 35 scams, or 77.1% of all
scam incidents. They alone represent 48.2% of the entire 56-incident
dataset.

exchange_scam is particularly dominant. The underlying cases repeatedly
involve fraudulent investment or trading platforms, fabricated balances
or profits, withdrawal restrictions, additional tax or verification
payments, and platforms introduced by online contacts.

**Hack Taxonomy**

  -----------------------------------------------------------------------------
  **Hack Subtype**             **Incidents**   **Share of    **Share of All
                                               Hacks**       Incidents**
  ---------------------------- --------------- ------------- ------------------
  wallet_software_exploit      5               55.6%         8.9%

  social_engineering_hack      2               22.2%         3.6%

  fake_app_or_extension_hack   1               11.1%         1.8%

  spyware                      1               11.1%         1.8%

  Total                        9               100.0%        16.1%
  -----------------------------------------------------------------------------

More than half of hack-classified incidents fall under
wallet_software_exploit. However, several of these records explicitly
lack a confirmed initial compromise vector. The numerical concentration
therefore does not necessarily indicate that five independently
confirmed software vulnerabilities occurred.

This distinction matters when interpreting the hack dataset:
classification reflects the canonical taxonomy available to the ingest
process rather than proof of a specific technical exploit in every case.

**User Mistake Taxonomy**

  ------------------------------------------------------------------------------
  **User Mistake         **Incidents**   **Share of User      **Share of All
  Subtype**                              Mistakes**           Incidents**
  ---------------------- --------------- -------------------- ------------------
  wrong_network          6               50.0%                10.7%

  lost_wallet_access     3               25.0%                5.4%

  wrong_address          2               16.7%                3.6%

  seed_phrase_exposure   1               8.3%                 1.8%

  Total                  12              100.0%               21.4%
  ------------------------------------------------------------------------------

Transfer compatibility is the clearest user-error cluster. wrong_network
alone represents half of all user mistakes and 10.7% of all incidents.

Several of these cases involve a more precise operational failure than
the subtype name alone conveys: the destination platform supported the
blockchain but did not support that specific asset on that blockchain.
This is an important recurring distinction for prevention content.

Combining wrong_network and wrong_address, 8 of 12 user mistakes ---
66.7% --- occurred during asset transfer execution.

**Taxonomy Concentration**

  ----------------------------------------------------------------------------------
  **Rank**   **Incident     **Incident Subtype**         **Incidents**   **Share**
             Type**                                                      
  ---------- -------------- ---------------------------- --------------- -----------
  1          scam           exchange_scam                17              30.4%

  2          scam           social_engineering           10              17.9%

  3          user_mistake   wrong_network                6               10.7%

  4          hack           wallet_software_exploit      5               8.9%

  5          user_mistake   lost_wallet_access           3               5.4%

  6          scam           job_scam                     2               3.6%

  6          scam           phishing                     2               3.6%

  6          scam           romance_scam                 2               3.6%

  6          hack           social_engineering_hack      2               3.6%

  6          user_mistake   wrong_address                2               3.6%

  11         scam           airdrop_scam                 1               1.8%

  11         scam           token_launch_scam            1               1.8%

  11         hack           fake_app_or_extension_hack   1               1.8%

  11         hack           spyware                      1               1.8%

  11         user_mistake   seed_phrase_exposure         1               1.8%
  ----------------------------------------------------------------------------------

The four largest subtypes account for 38 of 56 incidents --- 67.9% of
the entire dataset. The taxonomy is therefore highly concentrated rather
than broadly distributed.

**Classification Quality**

  ------------------------------------------------------------
  **Classification Warning**       **Incidents**   **Share**
  -------------------------------- --------------- -----------
  none                             29              51.8%

  taxonomy pressure resolved       18              32.1%

  insufficient detail to classify  8               14.3%
  confidently                                      

  mixed scam and technical vectors 1               1.8%

  Total                            56              100.0%
  ------------------------------------------------------------

Just over half of the records required no classification warning.

However, 18 incidents --- 32.1% --- required taxonomy-pressure
normalization. This is substantial and indicates that the deliberately
coarse taxonomy is regularly compressing more specific real-world
patterns into broader canonical categories.

A further 8 incidents --- 14.3% --- lacked enough information for
confident classification. These are concentrated particularly among
unexplained wallet-drain cases.

Taken together, 27 of 56 records --- 48.2% --- carry some form of
classification warning. This does not mean those records are invalid; it
does indicate that nearly half of the batch exercised ambiguity or
normalization handling.

**Source Distribution**

  -------------------------------------------
  **Source**      **Incidents**   **Share**
  --------------- --------------- -----------
  Reddit          50              89.3%

  X               4               7.1%

  The Standard    1               1.8%

  Greekreporter   1               1.8%

  Total           56              100.0%
  -------------------------------------------

The dataset is overwhelmingly Reddit-derived. This provides strong
access to first-person incident narratives and detailed user behavior
but should be considered when interpreting the dataset as an indicator
of the broader crypto threat environment: 89.3% of observations
originate from one source ecosystem.

**Key Findings**

  -----------------------------------------------------------------------
  **Finding**                    **Result**
  ------------------------------ ----------------------------------------
  Dominant incident class        Scam --- 35 incidents --- 62.5%

  Dominant subtype               exchange_scam --- 17 incidents --- 30.4%

  Second-largest subtype         social_engineering --- 10 incidents ---
                                 17.9%

  Largest user-mistake pattern   wrong_network --- 6 incidents

  Largest hack classification    wallet_software_exploit --- 5 incidents

  Scam concentration             exchange_scam + social_engineering =
                                 77.1% of scams

  Transfer-error concentration   wrong_network + wrong_address = 66.7% of
                                 user mistakes

  Top-four subtype concentration 38 incidents --- 67.9%

  Records without classification 29 --- 51.8%
  warning                        

  Records with taxonomy pressure 18 --- 32.1%

  Records with insufficient      8 --- 14.3%
  classification detail          
  -----------------------------------------------------------------------

The clearest signal from these 56 incidents is that the principal threat
remains deception rather than purely technical compromise. Scam
incidents outnumber hacks almost four to one, and the two dominant scam
categories center on fraudulent platforms and interpersonal
manipulation.

A second strong signal is operational: asset/network compatibility
remains a recurring preventable failure. The wrong-network cases show
that users frequently understand the destination address but fail to
verify the complete asset + blockchain combination supported by the
receiving platform.

The third signal concerns taxonomy governance. exchange_scam is carrying
a very broad range of fraudulent trading and investment-platform
narratives. The 18 taxonomy-pressure warnings confirm that this
compression is occurring frequently. Under the current locked taxonomy
this is functioning as intended, but exchange_scam should remain a
category to watch longitudinally for future governance review rather
than being split during production classification.

**Data Integrity**

  ------------------------------------------------------------------
  **Check**                                             **Result**
  ----------------------------------------------------- ------------
  Declared incident count                               56

  CSV row count                                         56

  Incident-count reconciliation                         Pass

  SHA-256 verification                                  Pass

  Duplicate incidents previously identified across CW33 0
  and CW34                                              

  Distinct incident records                             56

  Incident ID formatting anomaly                        1

  Classification types outside allowed taxonomy         0

  Classification subtypes represented                   15
  ------------------------------------------------------------------

One source record contains the incident ID INC-2026-08-09-8b0ba3b15d,
whereas the other IDs use the compact date form INC-YYYYMMDD-hash. The
report preserves the value exactly as present in the supplied CSV; it
has not been silently corrected.

**Ordered Incident IDs**

  -------------------------------------
  **No.**   **Incident ID**
  --------- ---------------------------
  1         INC-2026-08-09-8b0ba3b15d

  2         INC-20260809-41c904753b

  3         INC-20260809-03a5eb4a9b

  4         INC-20260809-b6338b29af

  5         INC-20260808-398210eeb1

  6         INC-20260808-bca174ffc0

  7         INC-20260808-76a1b29974

  8         INC-20260808-51ec2f7ebc

  9         INC-20260808-5d93fe2d29

  10        INC-20260806-ec57885c67

  11        INC-20260808-c9c6f3e794

  12        INC-20260808-5d71be7af4

  13        INC-20260809-1806e76b38

  14        INC-20260811-a4a6a32754

  15        INC-20260811-5ce5c77884

  16        INC-20260811-c28a6dfa89

  17        INC-20260811-214f2536f7

  18        INC-20260811-000e496665

  19        INC-20260810-85c971e6e5

  20        INC-20260810-b2458d7410

  21        INC-20260813-1e651889e2

  22        INC-20260813-1497f813a1

  23        INC-20260813-301cd5a29f

  24        INC-20260813-9dbfb39a41

  25        INC-20260813-deb76cf289

  26        INC-20260813-494439bf9f

  27        INC-20260813-a65d1e5b68

  28        INC-20260813-926e654dcc

  29        INC-20260813-e0ba995ab8

  30        INC-20260813-63cbf1f521

  31        INC-20260812-4fb14ef14b

  32        INC-20260812-40178902f2

  33        INC-20260813-71b2cd9e3c

  34        INC-20260817-8c2f6fac46

  35        INC-20260816-f73fc357c6

  36        INC-20260816-a612650a5b

  37        INC-20260816-82cec60ccd

  38        INC-20260816-a7769b77cc

  39        INC-20260816-6488ced702

  40        INC-20260816-f604f93983

  41        INC-20260816-8dec692fe8

  42        INC-20260815-c67949a42b

  43        INC-20260814-4c7d9ec8ab

  44        INC-20260814-a03cb2598c

  45        INC-20260814-7a863b0fe9

  46        INC-20260818-59ec862a74

  47        INC-20260818-59ea13e6cd

  48        INC-20260818-da6b8a3db7

  49        INC-20260818-e8322f7756

  50        INC-20260818-ac4a7d7f46

  51        INC-20260818-9fddca4a89

  52        INC-20260817-2ad53c3b55

  53        INC-20260820-bcc0db9ecf

  54        INC-20260820-dea47463be

  55        INC-20260820-49f5bcd054

  56        INC-20260820-0a3cc16997
  -------------------------------------
