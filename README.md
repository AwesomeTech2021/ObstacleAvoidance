https://github.com/Jaeyoung-Lim/avoidance
<br>위 링크를 통해 PX4 Avoidance를 SITL 환경에서 시험준비 설정


<br>
<br><strong>스테레오 비젼카메라와 SITL을 이용한 Obstacle avoidance시뮬레이션 수행 과정</strong> 
<br>
 
 1.
 $ roslaunch local_planner local_planner_stereo.launch
 <br>local_planner 실행파일을 구동시킴 
 <br>시뮬레이션에서는 스테레오 카메라도 모의하기 위해서 local_planner_stereo.launch 도 함께 실행
 

2.
 $ rosrun image_view stereo_view stereo:=/stereo image:=image_rect_color
 <br>스테레오 카메라의 영상과disparity 가져오기
 
3.
 qgroundcontrol 을 실행한 후 미션맵에서 waypoint 설정
