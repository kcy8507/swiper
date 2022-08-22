# swiper

Swiper 라이브러리 연습

슬라이드를 쉽게 만들 수 있다.

여러가지 옵션들을 사용할 수 있다.(반응형도 여기서 조절!)

<script>       
    var swiper = new Swiper(".mySwiper", {         
      spaceBetween: 30,    // 슬라이드 사이 여백
      slidesPerView : 'auto', // 한 슬라이드에 보여줄 갯수        
      centeredSlides: true,    //센터모드        
      autoplay: {     //자동슬라이드 (false-비활성화)          
        delay: 2500, // 시간 설정          
        disableOnInteraction: false, // false-스와이프 후 자동 재생        
      },
        loop : false,   // 슬라이드 반복 여부
        loopAdditionalSlides : 1, 
        // 슬라이드 반복 시 마지막 슬라이드에서 다음 슬라이드가 보여지지 않는 현상 수정         
        pagination: { // 호출(pager) 여부          
          el: ".swiper-pagination", //버튼을 담을 태그 설정          
          clickable: true, // 버튼 클릭 여부        
        },         
        navigation: {   // 버튼          
          nextEl: ".swiper-button-next",           
          prevEl: ".swiper-button-prev",         
        },       
  });
    </script>
spaceBetween: 30, //
freeMode : false, // 슬라이드 넘길 때 위치 고정 여부
autoHeight : true,  // 현재 활성 슬라이드높이 맞게 높이조정
a11y : false, // 접근성 매개변수(접근성 관련 대체 텍스트 설정이 가능) 
resistance : false, // 슬라이드 터치 저항 여부
slideToClickedSlide : true, // 해당 슬라이드 클릭시 슬라이드 위치로 이동
allowTouchMove : true, // (false-스와이핑안됨)버튼으로만 슬라이드 조작이 가능
watchOverflow : true // 슬라이드가 1개 일 때 pager, button 숨김 여부 설정
slidesOffsetBefore : number, // 슬라이드 시작 부분 여백
slidesOffsetAfter : number, 



*display: none; 시 슬라이드 작동안하면 observer: true, observeParents: true,를 줘서 해당부모, 해당요소 감지하여 DOM변화시, 스와이퍼를 초기화시켜준다. (slick) variableWidth: true,
