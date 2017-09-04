--- 
# ENOVACOM Presentation

---
# Au programme

---
```
			protected void onSuccessfulAuthentication(HttpServletRequest request, HttpServletResponse response, Authentication authResult) throws IOException {
				super.onSuccessfulAuthentication(request, response, authResult);
				try {
					successHandler.onAuthenticationSuccess(request, response, authResult);
				} catch (ServletException e) {
					throw new RuntimeException(e);
				}
			}
```
