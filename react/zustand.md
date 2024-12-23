# zustand가 React 컴포넌트를 업데이트 할 수 있는 이유

zustand는 발행/구독 모델 기반으로 이루어져 있으며, 내부적으로 스토어 상태를 클로저로, 상태 변경을 구독할 리스너는 Set을 통해 관리한다.

use-sync-external-store를 이용한다.

- react 에서 외부 스토어를 구독할 수 있는 React Hook를 제공
  - 외부 스토어란 ?
    - zustand, redux 와 같은 상태 라이브러리 store
    - 변경 가능한 값과 해당 값의 변경 사항을 구독하는 이벤트를 제공하는 브라우저 API (DOM, Date, 전역 변수 ... )

https://ui.toast.com/weekly-pick/ko_20210812
