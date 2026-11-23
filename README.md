# 부산공장 월간 인원 스케줄

## GitHub/Vercel 배포
1. 이 폴더의 파일 전체를 GitHub 저장소 루트에 업로드합니다.
2. Vercel에서 해당 저장소를 Import합니다.
3. Framework Preset은 Vite, Build Command는 `npm run build`, Output Directory는 `dist`로 둡니다.
4. Environment Variables에 아래 두 값을 등록합니다.
   - `VITE_SUPABASE_URL`
   - `VITE_SUPABASE_PUBLISHABLE_KEY`
5. Deploy를 실행합니다.

## Supabase
- `public.schedules` 테이블과 RLS 정책이 필요합니다.
- Realtime publication에 `public.schedules`가 등록되어 있어야 합니다.
- 웹앱에는 service_role/secret key를 넣지 마세요.
