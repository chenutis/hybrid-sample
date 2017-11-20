# Hybrid Sample to showcase how the browser back button is broken when navigating from ng1 to ng2 and ng2 having a redirect

1. Navigate to 'AngularJS A'
   * Navigation works fine. Title should be a/ng1
2. Click on 'Redirect to b/ng2'
   * Navigation works fine. Title should be b/ng2
3. Click the browser back button
   * The title updates to 'a/ng1' (Good) but the page still reads: 'ANGULAR REDNDERED b/ng2'
   * Right click on the browser back button and we see two entries for a/ng1 at the top of the stack

At this point it seems like the redirect is not properly handled when transitioning from ng1 to ng2


