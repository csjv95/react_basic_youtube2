# Youtube 2

## Youtube Search

## Youtube list

### setp 1
fetch를 통해 get 방식으로 youtube 데이터를 가져와서 videos에 담아 VideoList 컴포넌트에서 map을 활용하여 전달받은 props.videos를 VideoItem 컴포넌트에 video로 넘겨주어 렌더링을 한다

* Detail

  * const [videos, setVideos] 선언하고 useState([]) 함수를 통해 videos는 []값을 전달 받고 setVideo는 리엑트 useState에서 제공하는 videos의 값을 업데이트할 수 있는 함수를 할당 받는다 
  * VideoList 컴포넌트에 videos([])를 전달
  * useEffet로 컴포넌트가 마운트되면 fetch가 실행되며 setVideos함수 호출하여 값을 할당한다
  * videos에 새로받은 값으로 업데이트한다
  * 업데이트된 videos값이 VideoList로 전달된다
  * VideoItem 값에 전달된다

### step 2
앞에서와 같이 화면에 title을 출력 해봤다면 다른 것도 어렵지 않습니다! fetch를 통해 받아온 데이터를 각각에 컴포넌트에 원하는 방식으로 보여주면 됩니다

* Detail
  * Youtube에서 받아온 props인 viedos의 데이터를 바탕으로 화면에 보여준다
  * videos에 있는 snippet.(title, thumbnails, channelTitle...)등등 원하는데이터를 보여준다
  * 계획한대로 css스타일링을 해준다

## Environment Variables
.env