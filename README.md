# BJPS Admin Sites

This repository publishes the standalone activity office annual work plan website from `public/index.html`.

The deployed site stores editable data in the browser localStorage. Use the built-in JSON backup before changing computers or browsers.

## Bojia Attendance Workflow

The attendance app is maintained in `public/rollcall.html`.

- Admin `159/159` sees `課照班點名` with all after-care class totals and total absence count.
- After-care teacher `111/111` starts at `課照班老師點名` with the selected grade-group roster and absence count.
- Admin `159/159` sees `16:10 社團點名` with today's club totals and total absence count.
- Each club teacher has an individual account that starts at only that teacher's `16:10 社團老師點名` roster and can switch to the independent `社團老師請假` page from the left navigation.
- After-care and club attendance share the same records across roles; only the labels and summary scope change.
- In the admin after-care and club pages, `今日總缺席` is gray text when the count is 0 and a red detail button when the count is 1 or more.
- The absence detail dialog is read-only and shows only: 課照/社團, 班級, 學生, 狀態.
- Each club teacher submits leave requests only for the assigned club from the independent `社團老師請假` page, chooses the leave date directly, and selects either `安排代課` or `本日課程延後至期末補課週`.
- Pending and rejected teacher leave requests can be edited or deleted by the club teacher; editing a rejected request resubmits it as pending. Approved requests stay locked.
- Selecting `安排代課` shows `不需補課`; the teacher may submit before a substitute is confirmed, but the administrator can approve substitute teaching only after both the substitute teacher name and phone number are completed.
- Selecting `本日課程延後至期末補課週` shows the automatically suggested makeup date. Admin sees teacher leave requests at the bottom of `活動組追蹤` and can approve only the requested course handling method or reject the request for revision.
- Term-end makeup dates are only available after the club term: Monday through Thursday map to `2026/12/28` through `2026/12/31`.
- Friday clubs cannot be assigned automatic term-end makeup; the system shows `星期五社團無法期末補課，建議以代課安排。`
- Approved makeup requests hide the original-date club attendance table and show that the club should be taken on the makeup date.

### Club Teacher Accounts

The account and password are identical. The legacy shared account `121/121` is disabled.

| Day | Club | Account / Password |
|---|---|---|
| Monday | 桌球社（週一） | `12101 / 12101` |
| Monday | 陶藝（週一） | `12102 / 12102` |
| Monday | 烏克麗麗（週一） | `12103 / 12103` |
| Monday | 籃球社（週一） | `12104 / 12104` |
| Tuesday | 縫紉社(二) | `12201 / 12201` |
| Tuesday | 跆拳道(二) | `12202 / 12202` |
| Tuesday | 足球社(二) | `12203 / 12203` |
| Tuesday | 創意點心（週二） | `12204 / 12204` |
| Tuesday | 兒童美術(二) | `12205 / 12205` |
| Wednesday | 直排輪社（週三） | `12301 / 12301` |
| Wednesday | 打擊樂(三) | `12302 / 12302` |
| Wednesday | 街舞社（週三A） | `12303 / 12303` |
| Wednesday | 街舞社（週三B） | `12304 / 12304` |
| Wednesday | 游泳社（週三） | `12305 / 12305` |
| Wednesday | 弦樂A團(三) (合) | `12306 / 12306` |
| Thursday | 創意點心（週四） | `12401 / 12401` |
| Thursday | 游泳社（週四） | `12402 / 12402` |
| Thursday | 弦樂A團(四) | `12403 / 12403` |
| Thursday | 弦樂A團(四) (小) | `12404 / 12404` |
| Thursday | 弦樂A團(四) (大) | `12405 / 12405` |
| Thursday | 弦樂A團(四)(小中) | `12406 / 12406` |
| Thursday | 弦樂B團-中大提琴 | `12407 / 12407` |
| Friday | 創意捏塑(五) | `12501 / 12501` |
| Friday | 無人機（週五） | `12502 / 12502` |
