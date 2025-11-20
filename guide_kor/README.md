
## kubespray-offline을 이용한 폐쇄망 환경 클러스터 구축 (Cilium)


### 기존 kubespray-offline의 Cilium 배포 오류를 해결하고, 폐쇄망 환경 클러스터 구축 가이드



다음의 가상 환경을 기준으로 테스트 및 작성되었습니다.

가상화 플랫폼: VMware

운영체제 (OS): Rocky Linux 9.x (모든 노드 동일)

Kubespray 버전: 2.29.0

Kubespray-offline 버전: 2.29.0-0

 


### 본 가이드 테스트 사양


Bastion

8 vCPU, 4GB RAM, 150GB Disk



Control Plane

8 vCPU, 4GB RAM, 50GB Disk



Worker

8 vCPU, 4GB RAM, 50GB Disk



[중요] 환경 참고 사항:

Bastion 디스크: 위 가이드의 outputs 오프라인 번들(패키지, 이미지, 바이너리)은 약 35GB의 디스크 공간을 사용했습니다. 향후 업데이트 및 추가 이미지를 고려하여 Bastion 서버는 최소 50GB 이상의 디스크 공간을 확보해야 합니다.
