쿼리가 충분히 많으면 발생

max_prepare_stmt 대비 현재 prepare_stmt를 확인해야 한다.

트랜잭션에 실패할 수 있다. max_prepare_stmt 의 값을 늘려주면 해결된다. 