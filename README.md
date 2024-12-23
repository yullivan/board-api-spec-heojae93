# 게시판 생성
> POST /api/boards

# 게시판 목록 조회
> GET /api/boards

# 특정 게시판 조회
> GET /api/boards/{id}

# 특정 게시판 수정
> PUT /api/boards/{id}

# 특정 게시판 삭제
> DELETE /api/boards/{id}

# 게시글 생성
> POST /api/boards/{boardId}/posts

# 게시글 목록 조회 (특정 게시판 내)
> GET /api/boards/{boardId}/posts

# 특정 게시글 조회
> GET /api/posts/{id}

# 게시글 수정
> PUT /api/posts/{id}

# 게시글 삭제
> DELETE /api/posts/{id}

# 댓글 생성
> POST /api/posts/{postId}/comments

# 댓글 목록 조회 (특정 게시글 내)
> GET /api/posts/{postId}/comments

# 특정 댓글 조회
> GET /api/comments/{id}

# 댓글 수정
> PUT /api/comments/{id}

# 댓글 삭제
> DELETE /api/comments/{id}

# 댓글에 답글 생성
> POST /api/comments/{commentId}/replies

# 특정 답글 조회
> GET /api/comments/{commentId}/replies/{id}

# 답글 수정
> PUT /api/replies/{id}

# 답글 삭제
> DELETE /api/replies/{id}

# ENTITY
> 게시판 (class Board)  
> private Long id; (게시판의 고유 ID)  
> private String name; (게시판 이름)  
> private String description; (게시판 설명)  


> 게시글 (class Post)  
> private Long id; (게시글의 고유 ID)  
> private String title; (게시글 제목)  
> private String content; (게시글 내용)  
> private LocalDateTime createdAt; (게시글작성시간)  
> private LocalDateTime updatedAt; (게시글수정시간)


> 댓글 (class Comment)
> private Long id; (댓글의 고유 ID)  
> private String content; (댓글 내용)   
> private String author; (댓글 작성자)  
> private LocalDateTime createdAt; (댓글작성시간)  
> private LocalDateTime updatedAt; (댓글수정시간)  
 
