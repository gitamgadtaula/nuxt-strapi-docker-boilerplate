.<template>
  <div>
    <section class="bg-gray-50 dark:bg-gray-900">
      <div
        class="
          flex flex-col
          items-center
          justify-center
          px-6
          py-8
          mx-auto
          md:h-screen
          lg:py-0
        "
      >
        <a
          href="#"
          class="
            flex
            items-center
            mb-6
            text-2xl
            font-semibold
            text-gray-900
            dark:text-white
          "
        >
          <img
            class="w-8 h-8 mr-2"
            src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/logo.svg"
            alt="logo"
          />
          Meet app
        </a>
        <div
          class="
            w-full
            bg-white
            rounded-lg
            shadow
            dark:border
            md:mt-0
            sm:max-w-md
            xl:p-0
            dark:bg-gray-800 dark:border-gray-700
          "
        >
          <Form
            @submit="onRegister"
            class="p-6 space-y-4 md:space-y-6 sm:p-8"
            :validation-schema="schema"
          >
            <h1
              class="
                text-xl
                font-bold
                leading-tight
                tracking-tight
                text-gray-900
                md:text-2xl
                dark:text-white
              "
            >
              Create and account
            </h1>
            <div class="space-y-4 md:space-y-6">
              <div>
                <label
                  for="email"
                  class="
                    block
                    mb-2
                    text-sm
                    font-medium
                    text-gray-900
                    dark:text-white
                  "
                  >Your email</label
                >

                <Field
                  type="email"
                  name="email"
                  id="email"
                  class="
                    bg-gray-50
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-primary-600 focus:border-primary-600
                    block
                    w-full
                    p-2.5
                    dark:bg-gray-700
                    dark:border-gray-600
                    dark:placeholder-gray-400
                    dark:text-white
                    dark:focus:ring-blue-500
                    dark:focus:border-blue-500
                  "
                  placeholder="name@company.com"
                  required=""
                />
                <ErrorMessage class="text-rose-600" name="email" />
              </div>
              <div>
                <label
                  for="username"
                  class="
                    block
                    mb-2
                    text-sm
                    font-medium
                    text-gray-900
                    dark:text-white
                  "
                  >Username</label
                >

                <Field
                  type="text"
                  id="username"
                  name="username"
                  placeholder="john22"
                  class="
                    bg-gray-50
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-primary-600 focus:border-primary-600
                    block
                    w-full
                    p-2.5
                    dark:bg-gray-700
                    dark:border-gray-600
                    dark:placeholder-gray-400
                    dark:text-white
                    dark:focus:ring-blue-500
                    dark:focus:border-blue-500
                  "
                  required=""
                />
                <ErrorMessage class="text-rose-600" name="username" />
              </div>
              <div>
                <label
                  for="password"
                  class="
                    block
                    mb-2
                    text-sm
                    font-medium
                    text-gray-900
                    dark:text-white
                  "
                  >Password</label
                >

                <Field
                  name="password"
                  type="password"
                  id="password"
                  placeholder="••••••••"
                  class="
                    bg-gray-50
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-primary-600 focus:border-primary-600
                    block
                    w-full
                    p-2.5
                    dark:bg-gray-700
                    dark:border-gray-600
                    dark:placeholder-gray-400
                    dark:text-white
                    dark:focus:ring-blue-500
                    dark:focus:border-blue-500
                  "
                  required=""
                />
                <ErrorMessage class="text-rose-600" name="password" />
              </div>
              <!-- <div>
                <label
                  for="confirm-password"
                  class="
                    block
                    mb-2
                    text-sm
                    font-medium
                    text-gray-900
                    dark:text-white
                  "
                  >Confirm password</label
                >
                <Field
                  type="confirm-password"
                  name="confirm-password"
                  id="confirm-password"
                  placeholder="••••••••"
                  class="
                    bg-gray-50
                    border border-gray-300
                    text-gray-900
                    sm:text-sm
                    rounded-lg
                    focus:ring-primary-600 focus:border-primary-600
                    block
                    w-full
                    p-2.5
                    dark:bg-gray-700
                    dark:border-gray-600
                    dark:placeholder-gray-400
                    dark:text-white
                    dark:focus:ring-blue-500
                    dark:focus:border-blue-500
                  "
                  required=""
                />
              </div> -->
              <!-- <div class="flex items-start">
                <div class="flex items-center h-5">
                  <Field
                    id="terms"
                    aria-describedby="terms"
                    name="terms"
                    type="checkbox"
                    class="
                      w-4
                      h-4
                      border border-gray-300
                      rounded
                      bg-gray-50
                      focus:ring-3 focus:ring-primary-300
                      dark:bg-gray-700
                      dark:border-gray-600
                      dark:focus:ring-primary-600
                      dark:ring-offset-gray-800
                    "
                    required=""
                  />
                </div>
               <div class="ml-3 text-sm">
                  <label
                    for="terms"
                    class="font-light text-gray-500 dark:text-gray-300"
                    >I accept the
                    <a
                      class="
                        font-medium
                        text-primary-600
                        hover:underline
                        dark:text-primary-500
                      "
                      href="#"
                      >Terms and Conditions</a
                    ></label
                  >
                </div> 
              </div> -->
              <button
                type="submit"
                class="
                  w-full
                  text-white
                  bg-green-600
                  hover:bg-primary-700
                  focus:ring-4 focus:outline-none focus:ring-primary-300
                  font-medium
                  rounded-lg
                  text-sm
                  px-5
                  py-2.5
                  text-center
                  dark:bg-primary-600
                  dark:hover:bg-primary-700
                  dark:focus:ring-primary-800
                "
              >
                Create an account
              </button>
              <p class="text-sm font-light text-gray-500 dark:text-gray-400">
                Already have an account?
                <nuxt-link
                  to="/login"
                  class="
                    font-medium
                    text-primary-600
                    hover:underline
                    dark:text-primary-500
                  "
                  >Login here</nuxt-link
                >
              </p>
            </div>
          </Form>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { Form, Field, ErrorMessage } from "vee-validate";
import * as yup from "yup";
definePageMeta({ layout: "guest" });
const { register } = useStrapiAuth();
const router = useRouter();
const { $toast } = useNuxtApp();
const schema = yup.object({
  email: yup.string().required().email(),
  password: yup.string().required().min(8),
  username: yup.string().required(),
});
const onRegister = async (values) => {
  try {
    await register({
      email: values.email,
      username: values.email,
      password: values.password,
    });
    router.push("/login");
    $toast("Account created", "success", 2000);
  } catch (e) {
    console.log(e.error);
    $toast(e.error.message, "error", 2000);
  }
};
</script>

<style>
</style>