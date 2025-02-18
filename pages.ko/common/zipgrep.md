# zipgrep

> Zip 아카이브 내 파일에서 확장 정규 표현식을 사용하여 패턴 찾기 (`?`, `+`, `{}`, `()` 및 `|` 지원).
> 더 많은 정보: <https://manned.org/zipgrep>.

- Zip 아카이브 내에서 패턴 검색:

`zipgrep "{{검색_패턴}}" {{경로/대상/파일.zip}}`

- 각 일치 항목에 대해 파일 이름과 줄 번호 출력:

`zipgrep -H -n "{{검색_패턴}}" {{경로/대상/파일.zip}}`

- 패턴과 일치하지 않는 줄 검색:

`zipgrep -v "{{검색_패턴}}" {{경로/대상/파일.zip}}`

- 검색에서 Zip 아카이브 내 파일 지정:

`zipgrep "{{검색_패턴}}" {{경로/대상/파일.zip}} {{검색할/파일1}} {{검색할/파일2}}`

- 검색에서 Zip 아카이브 내 파일 제외:

`zipgrep "{{검색_패턴}}" {{경로/대상/파일.zip}} -x {{제외할/파일1}} {{제외할/파일2}}`
