# ACCA_2025
Autonomous Vihicle Project with ERP42 

## repo 소개
acca 팀 주요 코드(SLAM, Perception등 일부 코드 제외)

darknet 제외(사유:용량)

# 실행 방법
git clone https://github.com/beomseok3/ACCA_2025

cd /ACCA_2025

*의존성 파일 설치*

rosdep install --from-paths src --ignore-src -r -y

*msg 먼저 빌드해주기!!*

colcon build --symlink-install --packages-select adaptive_clustering_msgs

*msg 빌드 적용을 위한 소스*

. install/setup.bash

*전체 패키지 빌드*

colcon build --symlink-install

