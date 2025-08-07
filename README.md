# Onyx-Client-Archive
Most versions ever released of Onyx Client. Leaked bc the dev was annoying asf and the client is shit.
It has auth so that needs to be removed before using.

How to remove auth:

Go to net then integr then to onyx.class
Invert (or maybe delete idk) the following:

if (!HWIDManager.Companion.isAuthed(activeSystemId)) {
      ClipboardHelper.Companion.copyToClipboard(activeSystemId);
      throw new NotAuthedException(activeSystemId);
    } 
