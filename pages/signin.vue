<template>
  <section class="grid md:grid-cols-2">
    <div class="w-full h-screen bg-slate-100 hidden md:flex"></div>
    <div class="flex justify-center items-center h-screen">
      <div class="w-full max-w-screen-sm m-auto">
        <div
          class="border border-stone-200 rounded-lg w-2/3 flex flex-col mx-auto items-center p-6"
        >
          <div class="flex flex-col space-y-4 w-3/4">
            <p class="text-lg">Sign in</p>

            <article>
              <p class="text-gray-800 text-xs font-medium leading-6">
                Email address
              </p>
              <UInput
                name="email"
                appearance="white"
                size="sm"
                :trailing="false"
              />
            </article>

            <article>
              <p class="text-gray-800 text-xs font-medium leading-6">
                Password
              </p>
              <UInput
                name="password"
                appearance="white"
                size="sm"
                placeholder="- - - - - - -"
                type="password"
                :trailing="false"
              />
            </article>

            <article class="flex flex-row justify-between items-center">
              <div
                class="flex flex-row space-x-1.5 justify-between items-center"
              >
                <UCheckbox name="remember_me" />
                <span class="text-slate-700 text-sm font-medium leading-6">
                  Remember me
                </span>
              </div>
              <span class="text-slate-700 text-sm font-medium leading-6">
                Forgot password?
              </span>
            </article>

            <article class="py-4 flex flex-col gap-y-2">
              <UButton color="black" variant="solid" block>Continue</UButton>
              <hr class="my-2" />
              <UButton color="white" variant="solid" block>
                <UIcon name="i-devicon-google" />
                Continue with Google
              </UButton>
              <UButton color="white" variant="solid" block>
                <UIcon name="i-devicon-github" />
                Continue with Github
              </UButton>
            </article>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>
