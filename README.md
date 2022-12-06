# ktds-jcompnay-frontend

Pure HTML+CSS+JS

## WAS 서버 ip 변경 방법
 * 파일 오픈: ktds-jcompnay-frontend/js/custom.js
```javascript 
	$.ajax({
        url: 'http://localhost:8080/api/wasVer', // 해당 라인 ip변경
        type: 'GET',
    }).done((data, textStatus, jqXHR) => {
        $('.banner_taital').text('Web Version: '+data);
		console.log(data);

    }).fail((jqXHR, textStatus, errorThrown) => {
		$('.banner_taital').text('Not Found Web Version')
        console.log('실패')
    });
```
